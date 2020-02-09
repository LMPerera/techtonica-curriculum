# Intro to HTTP

### Projected Time

Approximately 2 hours

### Motivation

HTTP is the backbone of the web, for both human users and other programs (APIs)

### Specific Things To Learn

- What is the HTTP standard?
- HTTP Request
- HTTP Response
- HTTP Header
- HTTP Status Codes

### Materials

- [HTTP Crash Course](https://www.youtube.com/watch?v=iYM2zFP3Zn0) - _first 17 minutes are all that matter but feel free to watch the whole thing as it covers Postman_
-  b0rk's [Anatomy of an HTTP Request](https://twitter.com/b0rk/status/1145362860136177664/photo/1)


### Lesson

- Watch the crash course video above
- Ask the SEAM for a paper copy of the HTTP Zine by Julia  (b0rk)
- Work through the rest of the practice

### Guided Practice

#### Premade Node Web Server
Node has a library as `http.request`. It is called `http.server`.

- For a prebuilt version
- `npm install -g http-server`
- `http-server`
- This will start a web server that will serve files in the current directory
- Run it in one of your project folders, such as your portfolio
- It will announce that it started a server on two sockets. We'll cover that again in Networkin
- Open the location in your browser: `http://127.0.0.1:8080`

### Build Your Own Web Server

Tutorial to do it yourself:

- [Your First Note HTTP Server](https://blog.risingstack.com/your-first-node-js-http-server/)

Now make some requests against it with your favorite HTTP client library from above.

#### From the Command Line

Instead of using a browser, let's see what's happening underneath.

- `brew install telnet` if not installed
- format is `telnet <server> <port>` (note: it's not a colon like in a URL)
- `telnet www.google.com 80`
- It will connect and inform you of the escape character
- type `GET / HTTP/1.0` then enter twice. This is the smallest valid HTTP request
- A Google web server will spit out the Google home page

##### Questions
- Why do you have hit enter twice?
- Why does the 80 port not show up in the browser?


### Independent Practice

Class does this thing themselves with specific additional items. This could be alone, with a partner, or small group; but the idea is that it's less guided, more independent.

### Challenge

Apprentices can try to do this other thing. Ideally, they will be challenged to connect what they've learned to some previous knowledge or additional research.


### Check for Understanding

Sync up with your pair or another apprentice who is available and go through the following exercises.

#### Paper Request
- Your the client: on **paper** write out a basic HTTP request 
- Hand it to your pair. They are the *server*.
- If the request is valid, write out a valid response and give it back to them
- If the request is not valid, identify how to fix it.

#### How to know what is required?
If you're curious what each required piece is, check out this [simplified HTTP specification](https://www.jmarshall.com/easy/http/#requestline). The [complete spec](https://www.w3.org/Protocols/rfc2616/rfc2616.html) is huge and uses a formal mathematical language if you want to go down a rabbit hole.

### Supplemental Materials

![](https://http.cat/408.jpg)

- [HTTP Status Code Cats](https://http.cat/ =100px)
- [HTTPS explained with Carrier Pigeons](https://www.freecodecamp.org/news/https-explained-with-carrier-pigeons-7029d2193351/)
