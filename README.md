# .README : *Challenge 01-html-css*

# On-The-Job: Improving Accessibility and Efficiency in the Code for the HORISEON Website

## UPENN LPS Boot Camp

## Description: Goals, Approaches, Processes, Takeaways

Tasked with taking a scalpel to the Horiseon website main page, I reviewed the requirements of the job and then opened the web page itself, applying a critical eye to it, assessing whether there were any obvious aesthetic or physically structural issues that the naked eye could pick up. Getting a sense of what the Horiseon homepage was trying to accomplish, I next took a dive in to the code itself in Visual Studio Code, opening both the _index.html_ and _style.css_ files side-by-side on my monitor.

Keeping in mind that the central goals of the job were general accessibility as well as simplification, efficiency, and consolidation of the code, I read through both files numerous times. Each time reading through the pages’ code, I endeavored to look at the sections and lines more and more closely. My first time through reading through the code of any page, I like to skim across it quickly so as to take in the overall feel of the code, making mental notes of any glaring errors or misplaced elements, attributes, etc. By the second or third time through, I was already adding comments to myself in the html and css files, which I also summarized in a separate note-taking program, in order to begin ordering my thoughts so that I could begin re-ordering the code on the page.

In the _index.html_ file, there were numerous tags that were unassigned or otherwise out of place. For example, there were some _div_ tags that used both the _class_ and _id_ selectors, where only class selectors were needed.

However, for the most part, it was the formatting and styling of the page that seemed to require the most work, and so I immediately dove in the _style.css_ code to see where I could start trimming and consolidating.  I began with some of the observations I had made when I was merely looking at the website itself in Chrome, including font sizes that seemed inappropriate (mostly being too small for accessibility needs in some places). Also, I noted an issue in the styling of the main Header itself containing the company name, where the color of “seo” in “Horiseon” was not being adequately accentuated in contrast from the rest of the word (as the web designer was clearly trying to make a connection with the Search Engine Optimization acronym).

As there are only 3 linked menu at the top, it seemed logical to increase the size of their text for visibility, as there remained plenty of room on the blue bar across the top. While the 3 classes created by the 3 link options — .search-engine-optimization, .online-reputation-management, and .social-media-marketing — were necessary to distinguish in order to properly hyperlink them to their corresponding sections lower in the fold of the page, I was able to consolidate most instances in the _styles.css_ code where all 3 classes were being used in places where a single parent class (e.g. “header” and “benefits”) could be used instead, as the elements contained therein were identical. In another such location I simply used commas to separate the 3 classes enfolding a single list of children, rather than repeating the list 3 times in full.

Structurally, in terms of the priority of headers, combined with attempting to compose the information contained within the _styles.css_ code in a mostly chronological or linear fashion that roughly mirrored the _index.html_ code structure wherein its styles were executed. In simpler terms, the _h2_ header section of the page, which begins with _div class=hero_ and encompasses the main body text linked from the top menu, was mostly towards the bottom of the _styles.css_ sheet, even though there was an _h3_ section above it (and I added an _h4_ in the Footer, which had been mistakenly given an _h2_ heading tag at the very bottom).

In short, the Styles sheet needed condensing, shortening, great efficiency of language, and some plain old mass movement of text to align with Header priority and the general flow of the website. All class and other changes were then brought back to index.html and placed in the corresponding, appropriate places.

Ultimately, the major aesthetic and structural issue that remains so far unsolved in the code has mostly to do with resizing the web page or viewing it at vastly different resolutions. As that did not seem to be a major goal of this particular job, I decided against employing _flex_ and other such tools. In terms of fonts and text size, I erred on the side of overly large rather than overly small text and didn’t mess with the styling of the fonts, prioritizing readability and sizing differences that were less drastic (e.g. body text that was closer in size to header text than had previously been the case).

Finally, I made the main Horiseon logo clickable to _index.html_ because I think that should always be the case on websites, so you always know how to get to the homepage immediately regardless of where else on the site you find yourself.

There were some other minor tweaks and alterations, and I had to make two secondary passes to restructure, reorient, and in some cases remove my own changes. While the final product possesses a relatively small (though important) number of changes for a relatively small web page, my mistakes or oversights during my initial passes allowed me to experiment with elements, attributes, formatting, styling, and so forth; as well as observe the interplay of greater synergies between pieces of the code and between the html and css documents. It is difficult for me to judge how successful I was in this early phase of the course; but whatever errors in choices of code and its configuration made by the author are, I hope, lessons to be learned on the path.

##
## Installation

### What are the steps required to install your project? Provide a step-by-step description of how to get the development environment running.

##
## Usage

**Horiseon Website Before and After:** Comparison of original lower fold of website with smaller fonts and updated version with more accessibility-friendly larger fonts.

![alt text](/assets/images/lowerfold0.jpg)

![alt text](/assets/images/lowerfold2.jpg)

## Credits

I used the following programs either directly or indirectly to help with this project:

- [VS Code](https://code.visualstudio.com/)
- [Chrome](https://www.google.com/chrome/)
- [Ulysses](https://ulysses.app/)
- [Znote](https://znote.io/)
- [Typora](https://typora.io/)

The following websites were used and/or consulted to varying degrees:

- [GitHub](https://github.com/)
- [GitLab](https://about.gitlab.com/)
- [The Full-Stack Blog: Professional README Guide](https://coding-boot-camp.github.io/full-stack/github/professional-readme-guide)
- [Mozilla MDN Web Docs](https://developer.mozilla.org/en-US/)
- [W3Schools HTML Tutorial](https://www.w3schools.com/html/default.asp)

##  License

**MIT License**

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Copyright (c) 2023 thebizzle81 (Jesse F. Brenner)

![TheJBizzle](https://img.shields.io/badge/TheJBizzle-blue)

v01.2
