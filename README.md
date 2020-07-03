# Review Scrapper
<p>This is a web application to scrap or to get data(here reviews) from
 Flipkart site for whatever product you want. You can also save this data
 to your DB, you just have to make minimal changes.</p>
 
[click here](https://review-scrapper49.herokuapp.com) to see demo.

---
 
> Installation

<p>I used PyCharm IDE in this project. You can use any IDE like Jupyter Notebook,
VSCode or Spyder, it doesn't matter.</p>
This project is working in Python 3.6. You can install it from Python official website to download
 
[click here](https://www.python.org/downloads/release/python-365/)

I used some external libraries Flask, requests, BeautifulSoup etc. 
I wrote name of libraries with specific version in requirements.txt file.
To install all this libraries download requiremnts.txt and put this 
in your project folder and run this command line in terminal.

```sh
pip install -r requirements.txt
```

I just imported libraries in my basic python file.
```python
import os
from flask import Flask, render_template, request, jsonify
from flask_cors import CORS, cross_origin
import requests
from bs4 import BeautifulSoup as bs
from urllib.request import urlopen as uReq
```
>Web Development

Flask API is used here for web development or as a web framework. You can
also use Django here but I prefer Flask for small projects. For beautification
of web page CSS has been used named as main.css and style.css present in
static/css. HTML files are present in templates named as base.html, index.html 
and results.html .


