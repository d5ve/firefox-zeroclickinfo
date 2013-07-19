firefox-zeroclickinfo
=====================

Forked from: https://github.com/duckduckgo/firefox-zeroclickinfo

Edited to change the awesomebar search query from `&q=$SEARCHTERM` to the localised (for me) `?kp=-1&kl=uk-en&kad=en_GB&q=$SEARCHTERM`

This required editing `data/search.xml` and adding the new params to the XML.

Build (on mac) with:

    $ mkdir ~/dev_tools/
    $ cd ~/dev_tools/
    $ curl -O https://ftp.mozilla.org/pub/mozilla.org/labs/jetpack/addon-sdk-1.14.tar.gz
    $ tar xf addon-sdk-1.14.tar.gz
    $ cd addon-sdk-1.14
    $ bash
    $ source bin/activate 
    $ mkdir ~/src
    $ cd ~/src
    $ git clone https://github.com/d5ve/firefox-zeroclickinfo.git
    $ cd firefox-zeroclickinfo
    $ cfx xpi
    
Then install `~/src/firefox-zeroclickinfo/ddg_for_firefox.xpi` in your browser.

DuckDuckGo enhancements for Firefox.

This addon can

- add a handy DuckDuckGo toolbar button to your browser for easy access to !bang tags (removable). 
- add DuckDuckGo as your default search engine through the address bar, search bar and context right-click menu (reversible).
- show DuckDuckGo instant answers on Google/Bing (removable).



