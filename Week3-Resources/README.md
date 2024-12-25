# Week 3

This week you will be learning BeatifulSoup4 (short form - BS4). What is BS4 you ask? It is a library used to parse the HTML and XML documents and is used for automation. Whats automation? Making a machine do the task for you. Why do you want to automate things? Because humans don't like repetitive tasks. What tasks does BS4 help in? Finding information from some web page by just running one program. Well, actually you find the information and tell the scraper to get it for you whenever you want, however many times you want. You will write the program and get the information from the website. What kind of information?

Suppose there is a website which shows you the current stock prices. You can go to the website and look at the prices whenever you want. But suppose you want to keep track of the prices time to time to make a dataset from that. What do you do? Open the website time to time and copy the prices from the website into a file and make the dataset? No. You write a script for that. You make a webscraper that scrapes the required information from your favourite website and store it in the format you want to use it later.

I think you can see the point of a web scraper now.

There are two libraries which you will learn for this project - BS4 and selenium. We will learn BS4 this week.

In short, it is a parser for HTML and XML code. Whats a parser? https://stackoverflow.com/a/2933208/23518773 This answer explains it well.

For BS4, there is very less to read. You would be practicing more instead. Here is a list of tasks you can do with BS4: https://www.w3resource.com/python-exercises/BeautifulSoup/index.php Try to solve these tasks on the websites given here: https://webscraper.io/test-sites . Choose a site and write the script for it.

<b>Paths</b>. Have you ever tried `cat <file>` on a Ubuntu/Linux terminal? It prints out the contents in the file. Here `<file>` is actually path to that file. So for printing the contents of the file, you had to give `cat` the path of that file. Similar thing happens in a web scraper. You give a path to that element which contains the information that you need. And here the path is according to the HTML tags. These paths are called XPaths (XML Paths).

Your BS4 learning will be complemented with <b>Javascript</b>, the best language for an interactive website, the worst language while finding errors :)

One can say that the syntax of basic Javascript is a mixture of C++ and python, but it has a lot more things which are required for web design. <b>Events</b> being one. What are events you ask? For that, first you ask what is an interactive website? A website, where you don't just look at things/read them, but also give it inputs, which changes the things on the website. Examples of input to a website: pressing a button, scroll, hover the pointer over something, double click a button, pressing a key... All these are inputs. Javascript calls them events. Simple :))

## Resources
If you don't want to go through the <s>bs</s> motivation, here's a short list:<br>
 - <b>Requests</b> - https://www.w3schools.com/python/module_requests.asp . It will just be used for `requests.get()`.
 - <b>BS4 reference</b> - https://www.geeksforgeeks.org/implementing-web-scraping-python-beautiful-soup/ . Go through the code example to see how the structure of a webscraper is. Don't worry about the list of methods given there. There you will find some functions/terms. Get to know what they mean through searching on google. If you still don't get it, ask us.
 - <b>XPaths</b> - https://carpentries-incubator.github.io/lc-webscraping/02-xpath/index.html Actually, you can copy the XPath of some element using inspect element tool of browsers. But if you are working with an HTML document without opening it on the browser, you will need to know how to write XPaths of elements.
 - <b>BS4 problems (Must do)</b> - https://www.w3resource.com/python-exercises/BeautifulSoup/index.php . There's not much reading in for BS4. So you practice instead. On which website do you practice?
 - <b>Practice websites for scraping</b> - https://webscraper.io/test-sites . Choose any one website from this according to the problem and use `requests` module to get the HTML content and start scraping
 - <b> Java Script</b> - follow the following tutorials on https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Scripting:
     - What is JavaScript?
     - A First Splash Into JavaScript
     - TroubleShooting javaScript
     - Introduction to Events

## Some more <s>bs</s> motivation
After practicing BS4, you might notice that if an information appears on the website ("appears in the HTML code" would be more appropriate) after some event, then with BS4, you cannot get that information. Why? The problem is not with BS4. BS4 just parses the HTML code. The problem is from where it got the code. <b>Requests</b>. It got the code from requests. And requests got the code from when it did `requests.get(url)`. And that code it gets is from the time the url/website is reached (loaded). So you cannot interact with the website and get the required information. That's where <b>Selenium</b> comes to the rescue. But that's a story for next week :)
