# Introduction #

It is possible to use PWI to display pictures on Blogger. Below is a description.

Thanks to Norbert Bianchin for the description.

Note that this currently is a work in progress.

step #1: pwi integration (see pwi demo scripts)

  * Once blogger web site is created go to template and press edit HTML (I have used simple template with low customization)
  * insert mandatory css and js files, including files needed for the viewer (ColorBox or FancyBox). They must be inserted in the `<HEAD>` section, between the `<HEAD>` and `</HEAD>`. For faster upload you can use CDN server (ie cloudflare.com) or you can use the Google Code version (the example below uses release 2.0 of PWI, stored on Google Code):
```
    <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>

    <!-- These files are needed for ColorBox -->
    <link   href="http://pwi.googlecode.com/svn/tags/REL_2_0_0/js/jquery.colorbox/colorbox.css" rel="stylesheet" type="text/css"/>
    <script src="http://pwi.googlecode.com/svn/tags/REL_2_0_0/js/jquery.colorbox/jquery.colorbox-min.js" type="text/javascript"></script>

    <!-- These files are the PWI files -->
    <link   href="http://pwi.googlecode.com/svn/tags/REL_2_0_0/css/pwi.css" rel="stylesheet" type="text/css"/>
    <script src="http://pwi.googlecode.com/svn/tags/REL_2_0_0/js/jquery.pwi.js" type="text/javascript"></script>

    <!-- Needed for the Google Maps overview map -->
    <script type="text/javascript" src="http://maps.googleapis.com/maps/api/js?sensor=false"></script>   
    
```

  * save your template and check there is no error by displaying your blog and using Firebug or Chrome developer tool. Any error should be listed in console and associated to your blog url.