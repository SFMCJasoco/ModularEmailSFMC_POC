# ModularEmailSFMC_POC

Proof of concept for taking existing email template blocks and making it a little quicker to deploy campaigns with the right base template and configuration of AMPScript, using Excel as a catalyst.

The template elements within this were created in Milliner.App & I've included the HTML if anyone is interested.

---

The process is made up of a few parts:
        1. Define your template elements
        2. Define your AMPScript Variables
        3. An Excel Document or Google Sheet to pull it all together
        4. Pasting the Excel output into a template
        
---
1. Define your template elements
        In this example I've included 2 common template elements, a 2 spot with stacked image, text and cta button and a single placement with an image and text.
These were created in Milliner.App so check that out and see if it's helpful in your initial template component developments.

Each placement has a number of AMPScript placeholder requirements, in order to get the most value from the concept. So in this instance each:
Image URL
Image Alt text
Copy for the placement
Button Text
CTA Link for the button and image where appropriate

---
2. Define your AMPScript Variables
        In the HTML for the content blocks, you need to find where your AMPScript variables should go. For example: <a href="https://www.howtosfmc.com"> could become <a href="%%=V(@LeftSpotLink)=%%">
        So go through the HTML for your template and find the elements you want to be managed by a data source.
        
