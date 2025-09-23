---
content_type: page
description: This section provides examples of CORS and JavaScript snippets for use
  with the course projects.
learning_resource_types: []
ocw_type: CourseSection
parent_title: 'Project 1: Web Analytics'
parent_type: CourseSection
parent_uid: a34b2caf-5ee0-ad39-fbb0-ce7fdbaa7ac2
title: CORS and JS Snippets
uid: ceb361c5-b072-40aa-2ed1-db9fa52890cf
---

{{% resource_link a34b2caf-5ee0-ad39-fbb0-ce7fdbaa7ac2 "« Back to Project 1: Web Analytics" %}}

Same-Origin Policy and Cross-Origin Resource Sharing (CORS)
-----------------------------------------------------------

Modern browsers enforce a restriction called the same origin policy, which restricts the AJAX calls you can make. In general, you are only allowed to make requests to the same host and protocol as the request that originally served the page. A few methods exist to get around this limitation, including Cross-Origin Resource Sharing (CORS), a specification that is supported by modern browsers. When the browser detects a dynamic request for a resource on a different host or protocol, it first sends a special "pre-flight" request using the HTTP OPTIONS verb. The server can send back a list of domains (or a wildcard to indicate all domains) that can access that resource by using an HTTP header called `"Access-Control-Allow-Origin"`. If the browser determines that the origin is in that list, then the browser will allow the actual request to be sent. In Rails, you can edit your `config/routes.rb` file to process the OPTIONS request with a separate controller action (note that you will have to modify the routes to suite your application):

```
match "/restricted/resource" => "home#resource_preflight", :constraints => { :method => "OPTIONS" }
match "/restricted/resource" => "home#resource"
```

Then, in the controller, you may have something like this:

```
def set_cors_headers
   headers["Access-Control-Allow-Origin"] = "*"
   headers["Access-Control-Allow-Methods"] = "POST, GET, OPTIONS"
   headers["Access-Control-Allow-Headers"] = "Content-Type, Origin, Referer, User-Agent"
   headers["Access-Control-Max-Age"] = "3600"
end
```

```
def resource_preflight
   set_cors_headers
   render :text => "", :content_type => "text/plain"
end
```

```
def resource
   set_cors_headers
   render :text => "OK here is your restricted resource!"
end
```

Note that the CORS headers must be sent in both the response to the preflight OPTIONS request as well as the response including the actual resource.

AJAX
----

To make an asynchronous request in JavaScript, we must create a `XMLHttpRequest` object:

```
var xhr = new XMLHttpRequest();
```

Before making the actual request, you should define a handler function that will be called in response to various events. This handler will be called once for each of the four cases:

Now we can actually make the request:

```
xhr.open('GET', '/url/to/something', true);
xhr.send();
```

Here, the true argument means asynchronous. We could set this to `false`, and then the call would block until the request is received. Also, GET is the HTTP verb. You can also make POST requests (or any other type of request). If you were making a POST call, you might also want to pass data to the call to send, rather than the empty string.

A full snippet to send asynchronous requests might therefore look like:

```
var xhr = new XMLHttpRequest();
// We can ignore state change events if we're only interested in sending a request
// (and don't have any error handling mechanisms in place)
// xhr.onreadystatechange = function() {
// }
var params = "param1=/this/is/a/param¶m2=somethignelse";
xhr.open('GET', 'http://yoursite.com/url/to/something?' + params, true);
xhr.send();
```

Note that it's slightly different for POST requests due to how the data is passed:

```
var xhr = new XMLHttpRequest();
xhr.open('POST', 'http://yoursite.com/url/to/something', true);
var params = "param1=/this/is/a/param¶m2=somethignelse";
xhr.setRequestHeader("Content-type", "application/x-www-form-urlencoded");
xhr.send(params);
```

Alternatively, using jQuery, we can write this entire request as long jQuery is being included in the head of the document:

```
$.ajax({
   url:’/url/to/something’,
   success:function(data){
      console.log('We now have the complete response: ' + data);
   }
});
```

It should be noted that unless jQuery is already being used, this might be wasteful as it means downloading all of jQuery just to register the page visit.

{{% resource_link a34b2caf-5ee0-ad39-fbb0-ce7fdbaa7ac2 "« Back to Project 1: Web Analytics" %}}