# Introduction to HTTP

HTTP is the foundation of the World Wide Web. It's one of the most important protocols for developers to understand. If you master HTTP you'll have an advantage in the Web and APIs world. Whenever things get tough (security breaches, performance improvements, etc), having a deep understanding of how things work internally will make the difference.

HTTP is a stateless, text based protocol, which makes it easy to understand and debug.

## Client Server Architecture

HTTP was built on top of the Client-Server architecture. Clients will make requests to servers and servers will respond back whatever was required by the client.

In the case of HTTP, the most basic type of client we can identify is a traditional web browser. It's not the only client though. HTTP's power allows us to build _RESTful_ APIs on top of it. So any mobile application, smartwatch, smart TV, or any other device, can make HTTP requests to servers.

## Basic HTTP Request

A basic HTTP Request has the following form:

```
(1)              (2)                (3)
GET /advanced-python-programming HTTP/1.1

[BODY]
 (4)
```

Where:

1. Is the HTTP Method being used (more about this later)
2. Is the Path that we're trying to browse. Also known as the resource. Other examples might be `clients/`, `clients/1`, `clients/1/purchases`, etc.
3. Is the protocol version. There are different versions of HTTP, although HTTP 1.1 is the most widely used one.
4. After the first line (and leaving one blank line) we can put the body of the request.

## HTTP Methods

The first part of the request seen in our previous section was the _HTTP Method_ (also called _Verb_). This basically tells the server the "intention" that the client has with the given resource or path. For example, `GET` means that the client is trying to **read** that particular resource or path. In contrast, `POST` means the client is trying to **create** the resource or path. Here's a more comprehensive guide with HTTP Methods and a summary of each one:

* **GET**: Read a resource
* **POST**: Create a resource
* **PUT**: Update a resource
* **DELETE**: Delete a resource
* **HEAD**: Similar to `GET`, but without including the Body. Generally used to get information about the resource (response + headers).
* **PATCH**: Similar to `PUT`, is used to update a resource but with different semantics.
* **OPTIONS**: returns the HTTP methods that the server supports for the specified resource or path.

## Examples of Requests

Let's take a look at a few examples of requests:

##### Create a new tweet using Twitter's API

```
POST /tweets HTTP/1.1

{
  "content": "Good Flask Tutorial! #python #rmotr"
}
```

##### Get info from a tweet using Twitter's API


```
GET /tweets/839514567654924288 HTTP/1.1
```

##### Delete a tweet


```
DELETE /tweets/839514567654924288 HTTP/1.1
```

If you check closely the last two examples, you'll realize they're really similar. The only things that changes is the HTTP Method. Yet, they have completely different meanings (reading vs deleting). That's why it's so important to use the correct HTTP method for each request.

## HTTP Response


A basic HTTP Response looks something like:

```
  (1)      (2)
HTTP/1.1 200 OK

[BODY]
 (3)
```

Which includes:

1. The HTTP protocol version.
2. The status of the response (more about this in the next section)
3. The body of the response

For example, if you make a GET request to read Google's home page, you'll receive a response similar to:

```
HTTP/1.1 200 OK

<html>
  <head>
    <title>Google</title>
    ...
```

## HTTP Response Status Codes

The status code is a simple numeric code + a human readable message that lets clients quickly identify the status of the response. Just by looking at the status code, the client can quickly differentiate between a failed or successful response.

For example, all status codes starting with the number 2 (`2XX`) will mean successful responses. All the codes starting with a 4 (`4XX`) involve error responses. Just by checking this, the client can inform the user if the request was successful or not. Once the first quick look at the status code gives the client some general perspective of the response,

The status code serves as a quick summary, if the client desires more information it'll have to take a look at the response body or headers (more about headers later).

Here's a quick summary of the status codes categories:

* 2XX: Successful status codes
* 3XX: Redirection
* 4XX: Client Error (the client submitted an invalid request)
* 5XX: Server Error (not client's fault, the server has an error)

## Headers

Once we start developing more complex applications, the basic info that we can send and receive with requests and responses start to fall short. We need a more powerful way to send complementary information. HTTP Headers will allow us to send more info in our requests and responses. An HTTP Header is just an additional piece of information attached to either a request or response, it's a key-value pair. For example: `User-Agent:Mozilla/5.0` or `Content-Encoding:gzip`. There are many different types of headers, and you can even create custom ones for your own application.

### Example of Headers in a Request

```
GET /advanced-python-programming HTTP/1.1
Host: rmotr.com
Connection: keep-alive
Pragma: no-cache
Cache-Control: no-cache
User-Agent: Mozilla/5.0 (... truncated ...)
Accept: text/html,application/xhtml+xml, (... truncated ...)
Accept-Encoding: gzip, deflate, (... truncated ...)
Accept-Language: es-419,es;q=0.8,en;q=0.6,en-US;q=0.4
```

The server will use the information provided in those headers to serve a proper response to the client. For example, the header `Accept:` is a way the client has to communicate the server what types of formats it can read.

### Example of Headers in a Response

```
HTTP/1.1 200 OK
Server: nginx/1.4.6 (Ubuntu)
Date: Wed, 08 Mar 2017 23:30:23 GMT
Content-Type: text/html; charset=utf-8
Transfer-Encoding: chunked
Connection: keep-alive
Vary: Accept-Encoding
Content-Encoding: gzip
```

This will also allow the client to manipulate the content from the server in a better way. For example, the server is indicating to the client that the content type of the response is HTML (with the header `Content-Type:`).

You can always use your browser's devtools console to inspect the requests and responses sent and received.

Request to rmotr.com:

![An example of a request to rmotr.com](https://cloud.githubusercontent.com/assets/872296/23729232/6f9f4bec-043f-11e7-9626-561b129726dc.png)

Response from rmotr.com
![An example of a response from rmotr.com](https://cloud.githubusercontent.com/assets/872296/23729260/ae181688-043f-11e7-8aa8-ca31463a3ce1.png)

## An example of a Request-Response cycle

Let's see an example of a Request-Response cycle to wrap up this lesson. We'll use an example a little bit more complicated than what we've seen. We'll see how a URL shortening service is resolved. In our example, we're trying to fetch `bit.ly/rmotr-flask-tutorial`. In this case there will be three parts involved. The client will make a request to bit.ly, bit.ly will return the correct location of the result, and the client will finally reach its final destination.

**Step 1:** The request is started by the client with a request as follows:

```
GET /rmotr-flask-tutorial HTTP/1.1
Host: bit.ly
Accept: */*
```

**Step 2:** The server responds with something like:

```
HTTP/1.1 301 Moved Permanently
Server: nginx
Cache-Control: private, max-age=9
Location: https://rmotr.com/
```
In this case the status code is `301 Moved Permanently`. That tells the client that the resource doesn't live in `bit.ly/rmotr-flask-tutorial`, but somewhere else. That "somewhere else" is specified in the `Location` Header. The actual destination of `bit.ly/rmotr-flask-tutorial` is `https://rmotr.com/`.

**Step 3:**

The client sends its final request to `https://rmotr.com/` and displays the content.
