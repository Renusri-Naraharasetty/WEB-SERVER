# Developing a Simple Webserver
Name: Karthi Govindharaju
ID: ISAI005

# AIM:

Develop a webserver to display about top five web application development frameworks.

# DESIGN STEPS:

## Step 1:

HTML content creation is done

## Step 2:

Design of webserver workflow

## Step 3:

Implementation using Python code

## Step 4:

Serving the HTML pages.

## Step 5:

Testing the webserver
# PROGRAM:
```
from http.server import HTTPServer, BaseHTTPRequestHandler

content= """
<html>
<head>
</head>
<body>
<h1>welcome</h1>
</body>
</html>
"""
class HelloHandler(BasedHTTPRequestHandler):
    def do_GET(self):
        self.send-response(200)
        self.send_header('content-type','text/html;charset=utf-8')
        self.end_heardes()
        self.wfile.write(content.encode())

server_address=('',80)
httpdd=HTTPServer(server_address,HelloHandler)
httpd.serve_forever()
```

# OUTPUT:
![output](images/webserver1.png)

# RESULT:

The program is executed succesfully.
