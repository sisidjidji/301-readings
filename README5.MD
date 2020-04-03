# READ5

# Huruku:

to run our web server WITH HEROKU we need to follow those steps :

1. first step  instalation of Heroku
2. declare some variables:
    Exemple : var http = require("http");
          var fs = require("fs");
          var path = require("path");
          var mime = require("mime");

3. Create the package.json file and fill it with proper information.
4. It will create node_modules folder and place all the files inside of it. So, we resolve our dependencies and can return to our code.
5. We will now create send404() function. It will handle the sending of 404 error, which usually appears when requested file doesn't exist:
    Exemple:  function send404(response) {
              response.writeHead(404, {"Content-type" : "text/plain"});
              response.write("Error 404: resource not found");
              response.end();
              }
6. Now we will define sendPage() function. It first writes the header and then sends the contents of the file.
7. Now we'll define how our server will handle responses. This function will return the content of the requested file or the 404 error otherwise
8. create the HTTP server 
         var server = http.createServer(function(request, response) {
           var filePath = false;

           if (request.url == '/') {
           filePath = "public/index.html";
              } else {
            filePath = "public" + request.url;
             }

              var absPath = "./" + filePath;
             serverWorking(response, absPath);
          });

9. Now we need to start our server

          http.createServer(<some code here>).listen(3000)

10. Heroku sets a dynamically assigned port number to your app. That's why we need to handle all this mess with ports as it’s shown below

      var port_number = server.listen(process.env.PORT || 3000);