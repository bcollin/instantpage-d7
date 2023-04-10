Instant Page
------------

Prefetches a linked page's HTML on mouse hover or mouse down.

On an already fast-loading website, this creates a sense of immediacy.

On an already slow website, I am not sure how useful this is.

See https://instant.page .

This script prefetches, but does not prerender pages.


Requirements
------------

The visitor needs to have Javascript enabled.

Clean URLs must be enabled (admin/config/search/clean-urls).

(Clean URLs are what turn a path like '?q=node/2' into 'node/2'. Aliases are
what turn a path like 'node/2' into e.g. 'contact-us'.)


Installation
------------

 * Install as you would normally install a contributed Drupal module. Visit
   https://www.drupal.org/node/895232/ for further information.


Configuration
-------------

Currently configuration is neither possible nor required.

If you want to whitelist or blacklist links, you can use standard
Drupal hooks such as HOOK_preprocess_link() in your theme to do so.

See https://instant.page to find out how whitelisting and blacklisting
works and see this module's .module file for an example (e.g.
instantpage_preprocess_link()).


Troubleshooting
---------------

* This module seems to work out of the box in Chrome, but I had to change a
browser setting to get it to work in Firefox.

This was probably because I use Ublock Origin.

If you want to disable or enable prefetching in Firefox, see
https://support.mozilla.org/en-US/kb/how-stop-firefox-making-automatic-connections .

* This module blacklists the path 'user/logout'. Are there any others that
should be blacklisted?


Alternate solutions
-------------------

https://www.drupal.org/project/prefetch_cache (D8 only)

https://www.drupal.org/project/quicklink (prerenders)


Maintainers
-----------

Current maintainers:

 * Branko Collin (Branko Collin) - https://www.drupal.org/u/brankoc

Module based on the Instant.Page Wordpress plug-in
https://wordpress.org/plugins/instant-page/ by the script's author Alexandre
Dieulot.
