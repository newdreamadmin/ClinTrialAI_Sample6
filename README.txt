CLINTRIALAI STATIC HTML WEBSITE
===============================

This is the homepage of a future multi-page website.
It is plain HTML, CSS and JavaScript and requires no framework, Node.js,
npm command or compilation step.

FILES
-----
index.html       Homepage content and HTML structure
about.html       Mission, vision, company story, impact and values page
leadership.html  Leadership, principles, advisory and culture page
css/style.css    Shared theme, responsive layout, animations and transitions
js/site.js       Shared mobile menu and scroll interactions
images/          Logo and favicon
assets/images/   Optimized editorial photography used by the pages
web.config       IIS default-document and basic response-header settings

EDITING
-------
Edit the text and structure directly in index.html.
Edit colors, spacing, typography and animations in css/style.css.
Edit menu and scroll behavior in js/site.js.

The JavaScript file is not a framework or rendering engine. All visible
content is present directly in index.html. JavaScript is used only for the
mobile menu, scroll state, reveal effects, score animation and dialog behavior.
If JavaScript is unavailable, the page content remains readable.

FUTURE PAGES
------------
About and Leadership are the first additional pages. Other pages can be added at this same level, for example:

platform.html
retention-intelligence.html
enterprise.html
contact.html

Each future page can reuse css/style.css, js/site.js, images, the header and
the footer. No placeholder pages are included because the current phase is
homepage only.

IIS
---
Copy this folder's contents to the IIS site's physical directory. IIS will
serve index.html as the default page. Ensure the IIS Static Content and
Default Document features are installed.
