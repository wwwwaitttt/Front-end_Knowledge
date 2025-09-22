## Foreword

<!DOCTYPE html>is the first line declaration of an HTML document and has an important impact on the parsing and rendering of web pages. Understanding its function and principle will help to ensure that web pages are displayed consistently in different browsers and avoid compatibility problems caused by different document modes.


## <!DOCTYPE html>The role and mechanism

<!DOCTYPE html>is the Document Type Declaration (Doctype), which tells the browser that the current Document uses the HTML5 standard specification. It's not an HTML tag, but tells the browser what document standard to use to parse the page.


Due to the variety of HTML versions of early web pages, browsers entered different rendering modes according to Doctype:

- Standards Mode
  browsers parse and render pages according to the latest standards, ensuring better compatibility and consistency.
- Almost Standards Mode
  similar to standard mode, but compatible with some features.
- Quirks Mode
  in order to be compatible with old pages, the browser will imitate the rendering behavior of the old browser and ignore some standards, resulting in inconsistent layout and style performance.

HTML5 simplifies the Doctype declaration and only uses <!DOCTYPE html>, explicitly tell the browser to enable Standard mode and avoid entering weird mode.

If the Doctype is missing or the writing is incorrect, the browser may automatically enter weird mode, causing abnormal behavior such as CSS box model and layout calculation.

## Application recommendations

in web page development, be sure to declare at the beginning of the HTML file. <!DOCTYPE html>Ensure that the page is rendered in standard mode to avoid compatibility issues.

## Interview answer

<!DOCTYPE html>is the document type declaration for HTML5, telling the browser to parse and render the page according to the HTML5 standard. It ensures that the browser enables standard mode, avoids entering weird mode, and ensures consistent page layout and style performance. Missing or incorrect Doctype can cause browsers to use weird modes, affecting page compatibility and display.

## Summary

<!DOCTYPE html>although not an HTML tag, it plays a decisive role in the rendering mode of the web page. Proper use of Doctype is the foundation for ensuring compatibility and consistency of modern web pages, and is a must-have knowledge for every front-end developer.
