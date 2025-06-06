van Eyk Research
================

My role at van Eyk was software engineer/web developer, primarily for the financial research platform ‘iRate Online’.
At the time van Eyk were considered Australia's most respected financial research provider.
Clients and business relationships included BT, Coin (Macquarie), Oasis, OnePath, AMP, Count, Morningstar, Aspect Huntley, IRESS, FundData, Core Equity Services (CommSec), Bloomberg.


- [van Eyk Research](#van-eyk-research)
	- [iRate Online](#irate-online)
		- [Shares section](#shares-section)
		- [Quantitative Analysis](#quantitative-analysis)
	- [Fund and Share profiles](#fund-and-share-profiles)
	- [Share charts](#share-charts)
	- [van Eyk Conference website](#van-eyk-conference-website)
	- [Technologies](#technologies)
	- [Miscellaneous Graphics](#miscellaneous-graphics)



iRate Online
------------

<img src="image/iRate homepage.jpg" alt="iRate homepage" width="50%"/>

### Shares section

![iRate shares](<image/iRate_shares_1.jpg>)

### Quantitative Analysis

![Quantitative Analysis](image/iRate_Quant_image011.jpg)

Fund and Share profiles
-----------------------

[Fund Profile - 14175 original design.pdf](<pdf/Fund Profile - 14175 original design.pdf>)

A significant part of my work involved the automated production of fund and share reports (product profiles).

Features included:
* PDF and HTML generation
* On demand and batch creation
* Caching
* Custom client branding and layouts
* Delivery via SOAP, FTP and HTTP

PDFs were generated using XSL-FO and Apache FOP:

https://en.wikipedia.org/wiki/XSL_Formatting_Objects

https://en.wikipedia.org/wiki/Formatting_Objects_Processor

https://github.com/apache/xmlgraphics-fop

All charts and graphics were done in SVG, so the reports had very high quality images with very small file sizes.

Share charts were produced with a custom engine I wrote myself; fund charts were from an engine written by one of my colleagues.


Share charts
------------

![alt text](<shares/FXJ static.svg>)

I wrote the charting engine for the SVG share charts seen in the screenshots and reports.
At the time (early 2000s) no mainstream browser had a working SVG implementation; the only option was a surprisingly feature-complete browser plugin from Adobe (Adobe SVG Viewer).
Our users were directed to install the plugin.

For the charts viewed on the website I added a simple zooming animation using SMIL and EcmaScript.

<img src="shares/BHP.webp" alt="BHP Billiton LTD animation" width="50%"/>

There are working examples of the animated charts in the [shares](shares/) folder, however GitHub's CSP header prevents the scripts from running so they look a little broken when viewed directly (until I find a workaround):

	content-security-policy: default-src 'none'; style-src 'unsafe-inline'; sandbox

If you trust me, you can download these and run them locally in a modern browser to see the animation properly.
I had to clean up the SVG a little bit for modern browser compliance, but they're basically as presented back in the day.

Ref:
https://en.wikipedia.org/wiki/Synchronized_Multimedia_Integration_Language


van Eyk Conference website
--------------------------

<img src="image/Conference Website.jpg" alt="van Eyk Conference website" width="50%"/>



Technologies
------------
* ColdFusion
* HTML
* JavaScript
* CSS
* SVG
* SMIL
* XSL-FO
* Apache FOP
* Java
* Windows Server
* IIS
* HTTPS
* Microsoft SQL Server
* SOAP
* Eclipse
* Jira, Confluence etc (on-prem and OnDemand)
* Ubuntu
* VMWare
* Subversion
* Visual Sourcesafe


Miscellaneous Graphics
----------------------

<img src="graphics/vanEykLogo.svg" alt="van Eyk Logo" width="20%"/>
<img src="graphics/vanEykIcon.svg" alt="van Eyk Icon" width="20%"/>
<img src="graphics/iRateLogo.svg" alt="iRate Logo" width="20%"/>

<img src="graphics/vanEykSwirl.svg" alt="van Eyk Swirl" width="60%"/>

<img src="graphics/SvE.svg" alt="Stephen van Eyk" width="60%"/>


