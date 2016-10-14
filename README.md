# Web-Proxy-Development
This a project in the Network course in EURECOM with my teammate GONG Linxia

## Configuration before use

We set the Network configuration of proxy `MANUALLY`, and in this task we choose *Firefox* as example.

Configuration as follow:

* keep IP as default '', or explicitly '127,0,0,1'
* set port as 9090

This script works on Python 2.7.
You need to install OpenSSL to intercept HTTPS connections.


## Usage

Run as a script:

```
$ python proxy.py
```

The proxy runs on the port 9090 by default. To run on another port, type in  the port number as the first argument.

```
$ python proxy.py 9000
```

## Features
* Able to handle both HTTP and HTTPS requests
* Use seperate threads to support asynchronous tasks from each request
* Load from cache if the website is already opened before
