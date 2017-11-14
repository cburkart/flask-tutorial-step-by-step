Before we dig into how to create our website using Python and Flask we want to quickly explain to you the concepts behind the world wide web and the Internet.

The first concept that we want to explore is the client-server architecture 

When we talk about the world wide web we can identify two types of actors: clients and servers 

Our Flask application will act as one of these servers; it will receive requests from clients and respond with the proper data.

There's a wide variety of clients. The most common one is of course a simple web browser, but there are many more. 

For example if you're building a REST API using Flask we can have a mobile app as a client making requests to our application, or a smart TV, or even a car.

The web was built on top of the HTTP protocol. It's one of the most important concept to learn if you want to do the web development. It’s the foundation of the Internet.

HTTP is a stateless text-based protocol used to communicate [between] clients and servers.

That means that you will be able to see and read the information being transferred between them.

To explore HTTP in detail let's suppose you're browsing our Intro to Python course in our website rmotr.com 

The client initiates the request and that's basically initializing the communication by sending a request to the server .

The request has the following form:

From this request you can see we're specifying the path that we want to access in the given website in this case rmotr.com and then the protocol version that we’re using.

In this case we’re using HTTP 1.1 and this is standard so don’t worry much about it. 

The most important part of the request is the one where you see the get part. This is the HTTP method used by this request.

The client can specify different methods: GET, POST, PUT, PATCH, DELETE, HEAD, OPTIONS.  Each one of these methods will have a different meaning for the server.  

For example you can get a specified tweet and by that you're just reading that tweet or you can basically post a new tweet and that means that you're trying to create a new tweet.  

In the final case you can, for example, delete a given tweet by specifying that HTTP method.

We saw the server answer the client’s request with an HTTP response; a typical response will look similar to this one.

As you can see, the protocol version is included once again and as we told you before you don't have to worry much about it.

You also see the body of the response that contains the actual content of the site we’re browsing 

Finally we see the status code being returned. This is the most important part of the server response; in this case it's 200 OK.

The status code informs the client of the results of our request previously made. There are several status codes divided into the following categories. Usually by reading the first character you will identify the type of response that you're getting.  If you are dealing with a 200 status code, it will indicate that it’s a successful status code.

Let's see an example. Suppose we are trying to use a URL shortener like bit.ly 

In this case what is going to happen is that we will try to access bit.ly to get the particular path that we are trying to get.  bit.ly is actually shortening a URL that actually belongs to our server.

So what's going to happen is our web browser will send an initial request to bit.ly and the bit.ly will respond with a 301 status code.

In this case it will inform the actual location of the website we want to reach. Then our browser will just use that information in the location header to redirect to the correct place you were supposed to go.

Other examples could be a bad request: you're trying to post a tweet and you're forgetting some type of data or in other case you could just send a tweet with more than 140 characters. That will answer a 400 back from the server.

You can see a comprehensive list of HTTP responses on Wikipedia and we encourage you to take a look at all of them.

Finally, let's talk about HTTP headers. HTTP headers will allow clients and servers to include additional information.

When you were seeing requests and responses, you saw that the client has the ability to send the request method or verb (GET POST, for example) to include in the type of request that they were trying to do.

You also saw that the responses being returned by the server included a status code.

But that's not even enough information to communicate in today's web. 

So requests and responses can both include HTTP headers to augment the type of information that they are sending.

For example our request can, aside from informing the type of the request (in this case: GET), the path and the protocol version—as we saw that was a traditional request—it can also include additional information in the form of headers. In this case a host that is trying to reach the User-Agent that's basically a type of client and then for example they accept content type that is accepting that request. 

It's basically informing the server that it can accept just text/HTML content type; it's also informing the server with the Accept-Encoding header that it accepts content that has been zipped in order to minimize the size of the response. 

The response, for example, can include additional information like the server, the content type of the document that it's returning, and also the content length; it's basically the length in bytes that it's returning.

Again these are just headers. You can look them around, there are many headers and you can also create custom headers if you want to include some type additional information for your clients or your servers.

At this point we’re just scratching the surface of HTTP and the concepts behind how the web works. We would recommend you to keep learning about HTTP as it's one of the most important concepts for any good web developer.

Understanding HTTP in depth will give you the possibility to create better, faster, and more secure web apps.
