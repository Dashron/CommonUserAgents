# Common User Agents


The table below consists of a list of common user agent strings and the tools or libraries they are associated with.

### What is a User Agent String?
The [HTTP spec](https://tools.ietf.org/html/rfc7231#section-5.5.3) asks clients to identify themselves by providing a header called "User-Agent". This header's history is pretty [chaotic](http://webaim.org/blog/user-agent-string-history/),  but the [spec](https://tools.ietf.org/html/rfc7231#section-5.5.3) does a good job detailing how the header should actually work. 

This document lists some of the more common user agent strings that an API might encounter. If you find any are missing, feel free to add them via pull request or create an issue!

### Why is this useful?
To improve the onboarding experience of working with an API, the provider should offer libraries in their most popular languages. One easy way of identifying an API's most popular languages is by tracking the user agent strings of incoming HTTP requests.


| User Agent String | Source | Source Type  | Can be overriden? |
|-------------------|--------|--------------|-------------------|
| Guzzle/4.0 curl/7.21.4 PHP/5.5.7 | [Guzzle](https://github.com/guzzle/guzzle/blob/master/src/functions.php#L131) | HTTP library for PHP | Yes
| Guzzle/4.0 PHP/5.5.7         | [Guzzle](https://github.com/guzzle/guzzle/blob/master/src/functions.php#L131) | HTTP library for PHP | Yes
| python-requests/2.12.4 | [Requests](https://github.com/kennethreitz/requests/blob/master/requests/utils.py#L649-L655)| HTTP library for Python | Yes
