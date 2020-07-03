# Review Scrapper

1. About
1. Installation
1. Web Development
1. Programming
1. Deployment

>About

<p>This is a web application to scrap or to get data(reviews) from
 Flipkart site for whatever product you want. You can also save this data
 to your DB, you just have to make minimal changes.</p>
 
[click here](https://review-scrapper49.herokuapp.com) to see demo.

---
 
> Installation

<p>I used PyCharm IDE in this project. You can use any IDE like Jupyter Notebook,
VSCode or Spyder, it doesn't matter.</p>
This project is working in Python 3.6. You can install it from Python official website, to download
 
[click here](https://www.python.org/downloads/release/python-365/)

I used some external libraries Flask, requests, BeautifulSoup etc. 
I wrote name of libraries with specific version in requirements.txt file.
To install all this libraries download requiremnts.txt and put this 
in your project folder and run this command line in terminal.

```sh
pip install -r requirements.txt
```

 I just imported libraries in my basic app.py file.
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

>Programming

Requested data from flipkart url using 'uReq'. Used BeautifulSoup to make data readable.
To find <div> command of review section I used browser's Element Inspection tool.
By Iterating through the data I extracted some reviews and gave this back to html page as output.

>Deployment

I deployed my app on two platforms one is heroku and other one is Pivotal web services
They provide free deployment services with some restrictions to unlock all features
you have to pay them.
Pivotal Cloud Services give you 2GB memory space for free so if load will be
more on your site it may get crash.
Heroku Cloud platform gives you permission to upload 5 apps for free, and than
you have to pay for more.  

[click here](https://review-scrapper49.herokuapp.com/) to open app on heroku.

[click here](https://reviewscrapper-humble-puku-cm.cfapps.io/) to open app on pivotal.
 

<img src="https://resources.jetbrains.com/storage/products/pycharm/img/meta/pycharm_logo_300x300.png" alt="Pycharm" width="200"/> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3c/Flask_logo.svg/1200px-Flask_logo.svg.png" alt="Flask" width="200"/>       <img src="https://cdn.worldvectorlogo.com/logos/heroku.svg" alt="heroku" width="200"/>  <img src="https://run.pivotal.io/images/pws-header-logo_new.png" alt="heroku" width="300"/> 




