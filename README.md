CDIY Front-End Guidelines
===========

Performance Testing Guidance for Web Applications
-------------------------------------------------

Microsoft: [Performance Testing Guidance for Web Applications](http://perftestingguide.codeplex.com/downloads/get/17955 "Performance Testing Guidance for Web Applications") (To Read) 

Yahoo: [Complete List of Web Performance Best Practices and Rules](http://developer.yahoo.com/performance/rules.html "Complete List of Rules")

Google: [Web Performance Best Practices](https://developers.google.com/speed/docs/best-practices/rules_intro "Rules Introduction")

http://webdevchecklist.com/

Top 23 which can be tested with YSlow (as per Yahoo!'s Exceptional Performance team)

* Minimize HTTP Requests
* Avoid empty src or href
* Add an Expires or a Cache-Control Header
* Gzip Components
* Put StyleSheets at the Top
* Put Scripts at the Bottom
* Avoid CSS Expressions
* Make JavaScript and CSS External
* Reduce DNS Lookups
* Minify JavaScript and CSS
* Avoid Redirects
* Remove Duplicate Scripts
* Configure ETags
* Make AJAX Cacheable
* Use GET for AJAX Requests
* Reduce the Number of DOM Elements
* No 404s
* Reduce Cookie Size
* Use Cookie-Free Domains for Components
* Avoid Filters
* Do Not Scale Images in HTML
* Make favicon.ico Small and Cacheable
    
Yahoo's Firebug Extensions for Firefox:

YSlow analyzes web pages and suggests ways to improve their performance based on a set of rules for high performance web pages. YSlow is a Firefox add-on integrated with the Firebug web development tool. YSlow grades web page based on one of three predefined ruleset or a user-defined ruleset. It offers suggestions for improving the page's performance, summarizes the page's components, displays statistics about the page, and provides tools for performance analysis, including Smush.it™ and JSLint.

YSlow Firebug Extension: [Web Performance Best Practices and Rules](http://developer.yahoo.com/yslow/ "YSlow")

Google's Web Performance Best Practices

* Optimizing caching — keeping your application's data and logic off the network altogether
* Minimizing round-trip times — reducing the number of serial request-response cycles
* Minimizing request overhead — reducing upload size
* Minimizing payload size — reducing the size of responses, downloads, and cached pages
* Optimizing browser rendering — improving the browser's layout of a page
* Optimizing for mobile — tuning a site for the characteristics of mobile networks and mobile devices

Validate Document with minimal errors - [W3C Markup Validation Service](http://validator.w3.org "W3C")

Stanley Black & Decker Website Contractors Guidelines 
-----------------------------------------------------

1. **File Naming Conventions**

Rule #1: Avoid using special characters in a file name. \ / : * ? “ < > | [ ] & $ , .  
Rule #2: Use underscores instead of periods or spaces.  
Rule #3: Err on the side of brevity. Generally about 25 characters is a sufficient length to capture enough descriptive information for 
naming a record.   
Rule #4: The file name should include all necessary descriptive information independent of where it 
is stored.   
Rule #5: Be consistent.

*There will be exceptions.*  
One notable consideration is our PIM library and how the files are currently named there. 

Remember: this document is not going to apply absolutely to every situation; it should be used as a 
guide to encourage discussion in offices and workgroups to develop file-naming practices that work 
for best in those specific environments.

2. **Image Compression for Web Delivery**
