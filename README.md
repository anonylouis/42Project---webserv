# 42Project---webserv

In this c++ project we have to build a HTTP server from scratch !!  
- Only 3 methods are interpreted by the server : GET, POST and DELETE.  
- There are 3 cgi : a php-cgi, a python-cgi and a perl-cgi to read php, python and perl files.

The original subject from 42 Paris is [en.subject_webserv.pdf](https://github.com/anonylouis/42Project---webserv/blob/main/en.subject_webserv.pdf)

To run the project just ```make``` and :  
```./webserv [configuration file]```

A complete example of wath the server can do is available with the *conf_files/scale.conf* file !  

![start](https://github.com/anonylouis/42Project---webserv/blob/main/start.png)

There are some example of configuration files in the *conf_files* directory

## GET Request

You can test some get requests using curl :  

```curl 127.0.0.1:8000```

![get](https://github.com/anonylouis/42Project---webserv/blob/main/get.png)

## POST Request

You can test some post requests using curl :  

```curl -X POST -d "content" -H "Content-type: application/x-www-form-urlencoded" 127.0.0.1:8080/test.txt```  

Here a *test.txt* file containing "content" will be created  the root of 127.0.0.1:8080.  


## DELETE Request

You can test some delete requests using curl :  

```curl -X DELETE 127.0.0.1:8080/test.txt```  

The *test.txt* file will be deleted
