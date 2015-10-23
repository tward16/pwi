## Picasa Webalbum Integrator ##

PWI is a jQuery plugin for displaying pictures stored on Picasa on  web page. It has a lot of configuration options, to customize it according to the needs of your website. There is no need to edit the JavaScript files, configuration takes place in the HTML file, by overriding the default settings.

Some of the features of PWI:
  * Display multiple albums or just one single album.
  * Configurable thumbnail size for albums overview and album content.
  * Extensive filtering, using dates and keywords.
  * Integrated with SlimBox2 and FancyBox.
  * Show scaled images on website, with download link to original picture.
  * Fully translatable.
  * Show linked youtube video's.
  * Show map of where the photo was taken.

Take a quick look at the demo's [here](http://pwi.googlecode.com/svn/tags/REL_2_0_0/index.html)
or look at the Wiki




---

**latest version:** _2.0.0_ (last update: 29 Feb. 2012)


---


### Updates since last release ###

  * NEW:
    * Upgrade to jQuery 1.9.1, ColorBox 1.4.10 and FancyBox 2.1.4
    * Added callbacks at start and finish of PWI processing
    * Updated Demo 5, to show function of callbacks.
    * Removed Slimbox2 support, as this is not actively maintained anymore.

### Updates v2.0.0 ###

  * Some new features in this release:
    * Integrated ColorBox.
    * Added YouTube videos.
    * Show map with location where photo was taken.
    * Upgrade to jQuery 1.7.1 and FancyBox 2.0.5
    * Configuration of FancyBox and ColorBox integrated into PWI configuration
    * Updated demos, Code can be viewed directly from the demo


### Updates v1.5 ###

  * NEW:
    * Added Permalink feature using Query parameters
    * Improved download link function, including extra option to control this
    * Optionally remove albums with type Blogger, Scrapbook and/or ProfilePhotos albums

  * FIXES:
    * Fixed alignment on albums overview page
    * [Issue 82](https://code.google.com/p/pwi/issues/detail?id=82): fixed issue with dots in Picasa account name
    * Fixed showPhotoDownload handling


Well, download the latest package http://code.google.com/p/pwi/downloads/list with the code and samples and start playing!

Any personal comments, remarks or other things you would like to say are welcome at jdiderik(at)gmail.com or borkhuis(at)gmail.com.
Please ask your questions at our community-group site [here](http://groups.google.com/group/pwi-en)


Like what you see, feel free to [donate](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=XG9GP6AGHYE9Y&lc=US&item_name=PWI&currency_code=EUR&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted)


### ABOUT ###

A no-refresh, ajax-ian, high-speed, simple to include, Picasa web album placement javascript library...

This javascript library enables you to place your Picasa Web Albums on your own site without the need of server side code and extensive programming knowledge.

### LINKS ###

  * Demo: http://pwi.googlecode.com/svn/tags/REL_2_0_0/index.html
  * Group: http://groups.google.com/group/pwi-en


---


### HOWTO ###

  * goto the downloads section
  * download the latest zip file
  * unzip the zipfile in the root of your site (will create a pwi folder)
  * open up the html file you want your gallery in
  * Find a div that has an ID or give it one to be the container of your gallery
  * Add (atleast) the following to your header:
```
    <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.3.2/jquery.min.js"></script>
    <link   href="css/pwi.css" rel="stylesheet" type="text/css"/>
    <script src="js/jquery.pwi.js" type="text/javascript"></script>

    <script type="text/javascript">
        $(document).ready(function() {
	    $("#container").pwi({
	        username: 'tester'
            });
        });
    </script>
```
  * change tester to your picasa account name (duh), this can be found when you goto [picasa webalbums](http://picasaweb.google.com/home) on google, and choose (after logging in) My Public Webalbums. Take a look at the url, and you'll notice something like: http://picasaweb.google.com/tester ... well, the last part is the username you want!

Enjoy!

---

### Current dependencies/tested with ###

The current version is tested with jQuery 1.7.1 & plugins:

  * jQuery (v1.7.1, [website](http://jquery.com))

And optionally uses:

  * jQuery BlockUI (v2.16 [website](http://malsup.com/jquery/block/#overview))
  * jQuery Slimbox2 (v2.02 [website](http://www.digitalia.be/software/slimbox2))
  * jQuery fancybox ()v2.05 [website](http://fancyapps.com/fancybox/))
  * jQuery ColorBox()v1.3.19 [website](http://www.jacklmoore.com/colorbox))



---


### roadmap ###
Future options might be:

  * Diplay video
  * Albums-view paging
  * Multiple accounts integration (now possible on 1 page but as multiple containers)
  * Display photo comments
  * PHP Extension for placing comments (probably not gonna happen)


**REMARK:** This script might only work if your files are on a webserver, although it works on my Mac with FF3. So upload to your website inside a directory called /pwi (or somewhere else)
If you don't have a webserver that you can place the files on, or need a simple local server?
Then try a webserver like http://www.lighttpd.net/