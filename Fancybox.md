﻿#summary PWI: Using Fancybox

# Introduction #

One of the ways to show the photo's is by using Fancybox (see http://fancyapps.com/fancybox/). PWI includes an unmodified version of the Fancybox scripts.

To use the Fancybox script the Fancybox JavaScript library needs to loaded. Use the following code in the header of your page to load the Fancybox library:

```

    <!-- This can be your local jquery lib, but why not have it hosted by Google -->
    <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.7.2/jquery.min.js"></script>

    <!-- These files are needed for FancyBox -->
    <link   href="js/jquery.fancybox/jquery.fancybox.css" rel="stylesheet" type="text/css"/>
    <script src="js/jquery.fancybox/jquery.fancybox.pack.js" type="text/javascript"></script>
    
    <!-- These files are needed to display the FancyBox buttons at the top, including slideshow control --> 
    <link href="js/jquery.fancybox/helpers/jquery.fancybox-buttons.css?v=2.0.5" rel="stylesheet" type="text/css"/>
    <script type="text/javascript" src="js/jquery.fancybox/helpers/jquery.fancybox-buttons.js?v=2.0.5"></script>

    <!-- These files are the PWI files -->
    <link   href="css/pwi.css" rel="stylesheet" type="text/css"/>
    <script src="js/jquery.pwi-min.js" type="text/javascript"></script>

    <script type="text/javascript">

      $(document).ready(function () {
        var settings = {
            username: 'tester',  <!-- REPLACE WITH YOUR PICASA NAME!!!! -->
            fancybox_config: {
                config_photos: {
                    loop: true
                },
                config_youtube: {
                    width: '50%',
                    height: '50%',
                }
            }
          };
        $("#container").pwi(settings);
      });

    </script>

```

Here the loop-option for photos is switched on and for YouTube videos the width and height is reduced to 50 percent.

Within fancybox\_config 4 different configuration sections are defined:

| Name | Description |
|:-----|:------------|
| config\_photos | Configuration options used when viewing photos |
| config\_youtube | Configuration options used when viewing YouTube videos |
| config\_maps | Configuration options for photo-maps. This is the map shown for one photo |
| config\_map\_overview | Configuration options for the overview map |

Within these sections specific configuration options can be set for Fancybox. These options will be used when showing specific item. For example, the default for photos is to show navigation (previous/next), for YouTube videos this is disabled.

See http://fancyapps.com/fancybox/ for more information on Fancybox and on the other configuration options.

# Demos #

All demos include a Fancybox demo, but there are also some demos available in this Wiki:
  * Go to [here](FancyBoxDemoLatest.md) for a demo using the latest and greatest version of PWI
  * Go to [here](FancyBoxDemoCurrent.md) for a demo using the latest released version of PWI