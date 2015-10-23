﻿#summary The Picasa Webalbum Integrator javascript library.
#labels Featured

# Introduction #

This javascript library allows you to include your own Picasa Webalbum(s) into
your own site. Your visitors will never know the photo's came from google.
(unless they see the loading/traffic to and from google :-)


# Details #

Well, first get the correct files on your server:

  * goto the downloads section
  * download the latest zip file
  * unzip the zipfile in the root of your site (will create a pwi folder)
  * open up the html file you want your gallery in
  * Find a div that has an ID or create one to be the container of your gallery
  * Add the following code and [includes](PwiRequirements.md) to your header:

```

<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js"></script> //-->This can be your local jquery lib, but why not have it hosted by google

<!-- These files are needed for !ColorBox -->
<link   href="js/jquery.colorbox/colorbox.css" rel="stylesheet" type="text/css"/>
<script src="js/jquery.colorbox/jquery.colorbox-min.js" type="text/javascript"></script>

<script src="js/jquery.blockUI.js" type="text/javascript"></script> //--optional, shows the loading-box, little overhead

<link href="css/pwi.css" rel="stylesheet" type="text/css"/> //--contains the css used by PWI, change the settings in this file to create your own skin
<script src="js/jquery.pwi.js" type="text/javascript"></script> //-- The actual script :-)

<script type="text/javascript">
    $(document).ready(function() {  //-- default jQuery call, do stuff when page is loaded
        $("#container").pwi({  //--specify your DIV's ID here
            username: 'tester'  //--REPLACE WITH YOUR PICASA NAME!!!!
        });
    });
</script>

```

See the [Configuring PWI](Configuration.md) page for more configuration options, and the Using-pages on how to install and use the different viewers.
