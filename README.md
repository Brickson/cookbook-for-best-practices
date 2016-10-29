# Brickson Performance Handbook

**This handbook can be used as a checklist for deployment, or as a development resource for starting new projects. 

**The Brickson Performance Handbook is updated regularly by our Bricksonites, but we welcome all contributions you can make.

## Assets Optimisation

### CSS

*	Have you checked your CSS syntax and efficiency?

*This should be taken care of by your build script, but if the script does not include a (Sass/S)CSS lint step this should be done manually, for instance in an online linter.

* Have you added all appropriate vendor prefixes?

*If something like Autoprefixer or PostCSS is not part of your build script or your or if your favourite CSS preprocessor does not take care of vendor prefixes for you, this can be done manually by using an online tool like Autoprefixer CSS Online. Also: make sure you know which prefixes are required in your project, e.g. know which browsers your project must support.

* Have you minified your stylesheets?

*If you are using SASS, you can let the compiler take care of that for you. Alternatively, you can configure your build script to do it for you, or use an online service.


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

*There is no excuse for invalid HTML, just use an HTML linter in your build project or [W3C's]:https://validator.w3.org/ online validator tool.

* Have you implemented rich snippets?

*Add rich snippets (for example: Schema.org) to your markup. This is great for uncle Google and his nephews, but more importantly users with assistive devices will have a better user experience. While you’re at it, why don't you check out the accessibility section of the BPH?

### Optimisation

* Have you minified your HTML?

*If your server is configured to automatically minify your HTML for you, you’re all set. If not, consider adding this to your build script.

## SEO & Performance Optimisation

* Does your application require Google Analytics, or other tracking tools?

## Miscellaneaous

* Have you cleaned up any development code and/or databases?

*Like, for instance, have you made sure that no test accounts like admin/admin exist in your database? (Yes. It happens.)
