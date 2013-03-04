CDIY Front-End Guidelines
===========

Stanley Black & Decker Website Guidelines for Contractors.
-----------------------------------------------------

This is a living document and will be updated often with new requirements as new best practices and technologies emerge.

**1a. File Naming Conventions**
 
Our team tends to use Camel case for naming files.
The first letter of the filename is lowercase and the first letter of each subsequent concatenated word is capitalized. 
For example: backColor

Rule #1: Avoid using special characters in a file name. \ / : * ? “ < > | [ ] & $ , .  
Rule #2: Use underscores instead of periods or spaces.  
Rule #3: Err on the side of brevity. Generally about 25 characters is a sufficient length to capture enough descriptive information for 
naming a record.   
Rule #4: The file name should include all necessary descriptive information independent of where it 
is stored.   
Rule #5: Be consistent and use common sense.

*There will be exceptions.*  
One notable consideration is our PIM image library and how the files are currently named there. 

Remember: this document is not going to apply absolutely to every situation; it should be used as a 
guide to encourage discussion in offices and workgroups to develop file-naming practices that work 
for best in those specific environments.

**1b. Folder Structure:**

Since we will be using Sitecore as our WCMS I have found a few links that outline some "best practices" from current Sitecore users that run multiple sites. 
[Sitecore: Multiple Site Support Done Right - Folder Structure](http://xpressivecode.com/2012/1/3/sitecore-multiple-site-support-done-right-folder-structure.aspx "Sitecore: Multiple Site Support Done Right - Folder Structure")



**2. Image Compression for Web Delivery**

Utilize [PNGCrush](http://sourceforge.net/projects/pmt/files/pngcrush/1.7.51/ "PNGCrush") for PNG images.

Utilize [JPEGtran](http://jpegclub.org/ "JPEGtran") for JPG images.

For site images, which tend to be computer-generated and will be cached for re-use between pages, tend towards png; For site content, which will often be page-specific and likely large and complex enough to mask lossy compression, tend towards jpg.  
PNG files should be run through PNGCrush to acheive the correct compression and colors you would expect for your design . In general, a site optimizing its content will want to crush all of its PNG images (by using batch-mode conversion), and pngcrush includes two options to support batch conversion. The first allows one to specify a new extension for converted images, which will be created in the same directory as the original:

    pngcrush -e -crushed.png foo.png foo2.png foo3.png foo4.png

This example crushes four images, foo.png through foo4.png, giving them the extension -crushed.png; thus the output names are foo-crushed.png, foo2-crushed.png, and so on. Such an approach is handy for casual use, since an alphabetical directory listing will (usually) list the original and crushed versions in pairs, allowing quick, after-the-fact inspection of the changes in file sizes. But because it involves renaming files, this is probably not the preferred approach for a web site. The alternative is pngcrush's -d option, which allows one to specify an output directory in which to place the crushed images:

    pngcrush -d crushed_images foo.png foo2.png foo3.png foo4.png

This example crushes the same four images, but leaves their filenames unchanged. The new versions will go in the crushed_images subdirectory, which will be created if it does not already exist.

**3. Commenting Code** 

 Refer to - [Successful Strategies For Commenting Code](http://www.particletree.com/features/successful-strategies-for-commenting-code/ "Successful Strategies For Commenting Code")


**4. Performance Testing Guidelines**

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

YSlow analyzes web pages and suggests ways to improve their performance based on a set of rules for high performance web pages. YSlow is a Firefox add-on integrated with the Firebug web development tool. YSlow grades web page based on one of three predefined ruleset or a user-defined ruleset. It offers suggestions for improving the page's performance, summarizes the page's components, displays statistics about the page, and provides tools for performance analysis, including Smush.it™ and JSLint.

YSlow Firebug Extension: [Web Performance Best Practices and Rules](http://developer.yahoo.com/yslow/ "YSlow")
 
**5. General Front-End Guidelines**

Google's Web Performance Best Practices

* Optimizing caching — keeping your application's data and logic off the network altogether
* Minimizing round-trip times — reducing the number of serial request-response cycles
* Minimizing request overhead — reducing upload size
* Minimizing payload size — reducing the size of responses, downloads, and cached pages
* Optimizing browser rendering — improving the browser's layout of a page
* Optimizing for mobile — tuning a site for the characteristics of mobile networks and mobile devices

Validate Document with minimal errors - [W3C Markup Validation Service](http://validator.w3.org "W3C")

**6. SEO Guidelines**

* Indicate page titles by using title tags
* Accurately describe the page's content
* Create unique title tags for each page
* Use brief, but descriptive titles
* Make use of the "description" meta tag
* Accurately summarize the page's content
* Use unique descriptions for each page
* Simple-to-understand URLs will convey 
content information easily
* Use brief, but descriptive filenames and alt text
* Supply alt text when using images as links
* Supply an Image Sitemap file
* Use heading tags appropriately

**7. Cross Browser Compliance Guidelines, Javascript Plugins Guidelines**
* Utilize [Twitter Bootstrap](http://twitter.github.com/bootstrap/index.html "Twitter Bootstrap") to create a sleek, intuitive, and powerful front-end framework for faster and easier web development and better cross-browser compliance.

Deciding On Which JavaScript Recipe Is Right For You? - [Which JavaScript Recipe Is Right For You?](http://coding.smashingmagazine.com/2012/12/14/which-javascript-recipe-is-right-for-you/#more-120645 "Which JavaScript Recipe Is Right For You?")

Don't include more than one framework unless you absolutely have to.

**8. W3C Validation Guidelines, Responsive Design/Markup Guidelines**

Validate Document with minimal errors - [W3C Markup Validation Service](http://validator.w3.org "W3C")

Responsive Design on a Budget - [Responsive Design on a Budget](http://clearleft.com/thinks/responsivedesignonabudget/ "Responsive Design on a Budget")

**9. Boilerplate Adoption Guidelines, Mobile Compliance (Video, HTML, etc.)**


-------------------------------------------------
Appendix: Performance Testing Guidance for Web Applications
-------------------------------------------------

Microsoft: [Performance Testing Guidance for Web Applications](http://perftestingguide.codeplex.com/downloads/get/17955 "Performance Testing Guidance for Web Applications") (To Read) 

Yahoo: [Complete List of Web Performance Best Practices and Rules](http://developer.yahoo.com/performance/rules.html "Complete List of Rules")

Google: [Web Performance Best Practices](https://developers.google.com/speed/docs/best-practices/rules_intro "Rules Introduction")

http://webdevchecklist.com/
