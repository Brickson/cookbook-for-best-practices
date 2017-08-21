# Brickson Deployment Checklist

**Use as a checklist for deployment, or as a development resource for starting new projects.**

**The Brickson Checklist for Deployment is updated regularly by our Bricksonites, but we welcome all contributions you can make.**


## Table of Contents

1. Assets
2. Markup
3. Accessibility
4. SEO & Performance Optimisation
5. Maintainability
5. Social Sharing
7. Miscellaneous (gots to have miscellaneous)

## Assets Optimisation


### CSS

*	Have you checked your CSS syntax and efficiency?

_This should be taken care of by your build script, but if the script does not include a (Sass/S)CSS lint step this should be done manually, for instance in an online linter._

* Have you added all appropriate vendor prefixes?

_If something like Autoprefixer or PostCSS is not part of your build script or your or if your favourite CSS preprocessor does not take care of vendor prefixes for you, this can be done manually by using an online tool like Autoprefixer CSS Online. Also: make sure you know which prefixes are required in your project, e.g. know which browsers your project must support._

* Have you minified your stylesheets?

_If you are using SASS, you can let the compiler take care of that for you. Alternatively, you can configure your build script to do it for you, or use an online service._


### JavaScript

* Have you minified your JS?

* Have you uglified your JS?

* Have you merged your script where possible?


### Images

* Have you optimised your images (png, jpg, svg, gif)?


### Fonts

* Are you loading your fonts asynchronously and progressively?

* Are you using icon fonts? If so have you optimised them by taking out all the icons that your project does not use?

### Video

/* To do */

## Markup

### Syntax

* Have you checked your HTML for validity?

_There is no excuse for invalid HTML, just use an HTML linter in your build project or [W3C's]:https://validator.w3.org/ online validator tool._

* Have you implemented rich snippets?

_Add rich snippets (for example: Schema.org) to your markup. This is great for uncle Google and his nephews, but more importantly users with assistive devices will have a better user experience. While you’re at it, why don't you check out the accessibility section of the BPH?_

### Optimisation

* Have you minified your HTML?

_If your server is configured to automatically minify your HTML for you, you’re all set. If not, consider adding this to your build script._

## Accessibility

* Have you added a skip link?

_Small effort, huge return. See: https://www.w3.org/TR/WCAG20-TECHS/G1.html_

* Do your images contain meaningful alt texts (where appropriate)?

_If you’re image has meaningful content to convey, make sure that the alt text can cover the image's meaning for those users that rely on a screen reader. If you’re image does not have a contextual meaning, or can be left out without impairing the legibility of the content, you are free to use an empty alt tag. You may however not omit it!_

* Can your interface be navigated by keyboard?

_Impaired users often rely on their keyboard to navigate a site. Make sure this is possible and that the tab ordering makes sense (applies to more than form elements!)_


## SEO & Performance Optimisation

* Does your application require Google Analytics, or other tracking tools?


## Maintainability

/* To do */


## Social Sharing

* Does (part of) your project require Open Graph support?

_/* To do - hints & example */_


* Does (part of) your project require support for sharing on Twitter?

_/* To do - hints & example */_


## Miscellaneous

* Have you removed/disabled all debug code?

* Have you implemented appropriate error handling?
_ For instance, 4## and 5## pages

* Have you disabled directory listing?

* Have you added a favicon and app icons?

_There are generators that can help you create them, for instance http://realfavicongenerator.net_

* Have you cleaned up any development code and/or databases?

_Like, for instance, have you made sure that no test accounts like admin/admin exist in your database? (Yes. It happens.)_

* Have you added (if necessary) tracking codes?

_Google analytics, charbeat, etc._

* Use the "nofollow" attribute for links in the comment field. This will deter spammers from targeting your site. By default, many blogging sites (such as Blogger) automatically add this attribute to any posted comments.

* Check the robot.txt, is Google (not) allowed to track the appropriate paths?
