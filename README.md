# Common User Agents


The table below consists of a list of common user agent strings and the tools or libraries they are associated with.

### What is a User Agent String?
The [HTTP spec](https://tools.ietf.org/html/rfc7231#section-5.5.3) asks clients to identify themselves by providing a header called "User-Agent". This header's history is pretty [chaotic](http://webaim.org/blog/user-agent-string-history/), but the [spec](https://tools.ietf.org/html/rfc7231#section-5.5.3) does a good job detailing how the header should actually work. 

This document lists some of the more common user agent strings that an API might encounter. If you find any are missing, feel free to add them via pull request or create an issue!

### Why is this useful?
By tracking the user agent headers received by your API you can get a sense for what languages and libraries are used by your developers. If one language or library is used by many different API consumers, it might be worth supporting that language with an official API library.

### The list
**Note** I do not plan on listing out every possible version number, so you will need to substitue out the version numbers for wildcards.

| Source | Example User Agent String | Description  | Can be overriden by a developer? |
|-------------------|--------|--------------|-------------------|
| [Guzzle](https://github.com/guzzle/guzzle/blob/master/src/functions.php#L131) | "Guzzle/4.0 curl/7.21.4 PHP/5.5.7", "Guzzle/4.0 PHP/5.5.7" | HTTP library for PHP. The first one uses curl bindings, and the second uses native PHP HTTP functionality | Yes
| [Requests](https://github.com/kennethreitz/requests/blob/master/requests/utils.py#L649-L655) | python-requests/2.12.4 | HTTP library for Python | Yes
| [Curl](https://curl.haxx.se/) | curl/7.47.0 | An old, trusted HTTP request tool written in C. | Yes
| [Insomnia REST client](https://insomnia.rest/) | insomnia/5.0.20 | Insomnia is a cross platform HTTP request tool intended to help with API development  | Yes
| [Postman](https://www.getpostman.com/) | **TBD** | Postman is a popular cross platform HTTP request tool intended to help with API development | **TBD**
| [Paw](https://paw.cloud/) | **TBD** | A common mac-only HTTP request tool intended to help with API development | **TBD**

### Tools that do not provide default user agent strings
| Source | Description | Can be overriden by developer? |
|-------------------|--------|--------------|
| [PHP Curl](http://php.net/manual/en/book.curl.php) | PHP's standard curl bindings do not assign a default user agent | Yes
| [Node HTTP(S)](https://nodejs.org/dist/latest-v7.x/docs/api/http.html) | Node's standard request library for HTTP and HTTPS requests do not assign a default user agent | Yes



### Looking for....
**Libraries**
 - .Net
 - Java
 - Android
 - iOS
 - Go
 
 **Clients**
 - Postman
 - Paw
