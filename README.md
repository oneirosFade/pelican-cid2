# Cid2

Cid2 is a fork of Cid (by [Hendra](http://hndr.me)), which is a theme for the
[Pelican] static blog system. I've made a few changes that felt substantial 
enough to properly split off (instead of branch). I'll be making more 
substantial changes in the near future, so check the Depcrecated section
before deciding to use this theme over the original Cid. I might not be going
in a direction that you like.

## Features
* Disqus comment. `DISQUS_SITENAME` must be defined in configuration file.
* Responsive theme.
* Pagination.

## Deprecated Features (from Cid)
* Google Analytics. `GOOGLE_ANALYTICS` must be defined in configuration.
* Obfuscated Email. `CONTACT_EMAIL` must be defined in the configuration file. 
Javascript is required to view the email address.
* Landing Page template.

## Custom Footer Links
By default, the site footer will display the list of static pages configured 
on the site. To replace them with a list of links you want, specify a 
`USE_CUSTOM_MENU` configuration variable to be true, and create 
`CUSTOM_MENUITEMS` tuple in the `(Title, url)` format within your 
configuration file to contain the list of items you want to display. The URLs 
are specified relative to the `SITEURL`. Example:

    USE_CUSTOM_MENU = True
    CUSTOM_MENUITEMS = (('Blog', `blog`),
                 ('Contact', 'contact'),
                 ('Projects', 'pages/projects'))

#LICENSE
MIT

[pelican]: http://getpelican.com
