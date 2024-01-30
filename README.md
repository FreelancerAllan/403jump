# 403JUMP - HTTP 403 Bypass Tool

## Overview

403JUMP is a tool designed for penetration testers and bug bounty hunters to audit the security of web applications by attempting to bypass HTTP 403 (Forbidden) pages. It automates the process of sending various HTTP requests and headers to identify potential security vulnerabilities.


![403JUMP Image](https://github.com/trap-bytes/403jump/blob/main/static/tool.png)


## Features

- **Multiple Bypass Techniques Including:**  
	- Different HTTP Verbs
	- Different Headers
	- Path Fuzzing.
- **Customization:** Allows customization of headers and cookies for more targeted testing.
- **Concurrency:** Performs actions concurrently using goroutines for efficient and fast scanning.

## Install

```
go install github.com/trap-bytes/403jump@latest
```
## Usage:

```
403jump -h
```

This will display help for the tool. Here are all the arguments it supports.

```
Usage:
  403jump [arguments]

The arguments are:
  -t string    Specify the target URL (e.g., domain.com or https://domain.com)
  -f string    Specify the file (e.g., domain.txt)
  -p string    Specify the proxy URL (e.g., 127.0.0.1:8080)
  -c string    Specify cookies (e.g., user_token=g3p21ip21h; 
  -r string    Specify headers (e.g., Myheader: test
  -h           Display help

Examples:
  403jump -t domain.com
  403jump -t https://domain.com -p 127.0.0.1:8080
  403jump -f domains.txt
  403jump -c "user_token=hjljkklpo"
  403jump -r "Myheader: test"
```
