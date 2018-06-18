# wp-optimize-guide
How to optimize your Wordpress site

## Eliminate render-blocking JavaScript and CSS in above-the-fold content
1. Install and activate [Autoptimize](https://wordpress.org/plugins/autoptimize/) Plugin
1. Click `Autoptimize icon` on the `WP-admin bar` to go to the settings
1. Click `Show advanced settings`
1. Tick `Optimize HTML Code?` and `Optimize CSS Code?`
1. Click `Save Changes and Empty Cache`

## Optimize images
1. Scroll to the bottom of the pagespeed insights page
1. Find `Download optimized image, JavaScript, and CSS resources for this page.` and download assets
1. Reupload assets to their corresponding folders

## Leverage browser caching
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
