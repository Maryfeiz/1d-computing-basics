# 1D Computing Basics

Solution for 1D challenge.

## Description

The **index-generator** is a bash script which creats an index.html file representing a static web-page. 
By running a web-service (darkhttpd), clients will be able to see a table with existing images in the `images/` directory.  

## Usage

To generate an index.html file, run the following command:

```sh
./index-generator
```

The output of this script is a html file which should be served by a web service (darkhttpd):

```sh
darkhttpd . --port 12345
```

To see the result, open a browser and type `localhost:12345` , then press enter.

## Challenge Response

1. Exchange one of the images in the sample index.html and see if you can display that in the browser. Did you need to restart the server to do that? Why or why not? 
> Yes, we need to restart the server. The web server holds a copy of html file in cache memory, and any attempt to change the original source/images will not be displayed in the browser. In order to see the last changes, the web server requires to be restarted. 
---
2. How can you look up the process ID of your server? Document the command line used and the output.
> There are two ways to get the process ID of my server:
```sh
$ ps -A | grep darkttpd | grep -v grep | cut -d ' '  -f 1
41799

$ pgrep darkhttpd
41799
```

