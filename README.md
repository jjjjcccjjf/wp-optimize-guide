# WP Optimize Guide
How to optimize your Wordpress site

### Analyze your WP Site
1. Go to [google pagespeed insights](https://developers.google.com/speed/pagespeed/insights/) and have your website analyzed

## Common issues
After analyzing your site, you probably want to have a higher page speed score. Here are some guidelines on just how to do that.

### Eliminate render-blocking JavaScript and CSS in above-the-fold content
1. Install and activate [Autoptimize](https://wordpress.org/plugins/autoptimize/) Plugin
1. Click `Autoptimize icon` on the `WP-admin bar` to go to the settings
1. Click `Show advanced settings`
1. Tick `Optimize HTML Code?` and `Optimize CSS Code?`
1. Click `Save Changes and Empty Cache`

### Optimize images
1. Scroll to the bottom of the pagespeed insights page
1. Find `Download optimized image, JavaScript, and CSS resources for this page.` and download assets
1. Reupload assets to their corresponding folders
* (Optional) Download [Enable Media Replace](https://wordpress.org/plugins/enable-media-replace/) and then replace your assets one by one

### Leverage browser caching
1. Install and activate [W3 Total Cache](https://wordpress.org/plugins/w3-total-cache/)
1. On the `WP-admin sidebar` hover over `Performance` and then click `General Settings`
    1. Tick `Page cache` option
    1. Click `Save Settings & Purge Caches`
1. On the `WP-admin sidebar` hover over `Performance` and then click `Browser Cache`
    1. Tick `Set Last-Modified header`
    1. Tick `Set expires header`
    1. Tick `Set cache control header`
    1. Tick `Set W3 Total Cache header`
    1. Click `Save Settings & Purge Caches`
    
#### Extra notes
* External javascript cannot be cached (such as `analytics.js` and google tag manager's js)
* It is recommended not to minify JS. It might break your site. Oh, don't believe me? Try it.
* Page score updates are not instantaneous, so you better wait for a bit before you analyze again.
