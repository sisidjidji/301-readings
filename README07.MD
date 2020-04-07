# Read7:


## API's: 


- SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!

 - A request can be initiated by invoking the appropriate method on the request object, then calling .then() (or .end() or await) to send the request

 - HTTP method may also be passed as a string.

 - Absolute URLs can be used. In web browsers absolute URLs work only if the server implements CORS.

 - The Node client supports making requests to Unix Domain Sockets:

                  // pattern: https?+unix://SOCKET_PATH/REQUEST_PATH
                 //          Use `%2F` as `/` in SOCKET_PATH
                        try {
                        const res = await request
                        .get('http+unix://%2Fabsolute%2Fpath%2Fto%2Funix.sock/search');
                  // res.body, res.headers, res.status
                       } catch(err) {
                          // err.message, err.response
                                }

- You can also use the .query() method for HEAD requests. The following will produce the path /users?email=joe@smith.com.

- A typical JSON POST request might look a little like the following, where we set the Content-Type header field appropriately, and "write" some data, in this case just a JSON string.

- By default sending strings will set the Content-Type to application/x-www-form-urlencoded, multiple calls will be concatenated with &, here resulting in name=tj&pet=tobi

- SuperAgent formats are extensible, however by default "json" and "form" are supported. To send the data as application/x-www-form-urlencoded simply invoke .type() with "form", where the default is "json". This request will POST the body "name=tj&pet=tobi".

- As a short-hand the .type() method is also available, accepting the canonicalized MIME type name complete with type/subtype, or simply the extension name such as "xml", "json", "png", 