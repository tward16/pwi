﻿#summary PWI: Using Colorbox

# Introduction #

One of the ways to show the photo's is by using Colorbox (see http://jacklmoore.com/colorbox/). PWI includes an unmodified version of the Colorbox scripts.

To use the Colorbox script the Colorbox JavaScript library needs to loaded. Use the following code in the header of your page to load the Colorbox library:

```

    <!-- This can be your local jquery lib, but why not have it hosted by Google -->
    <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.7.2/jquery.min.js"></script>

    <!-- These files are needed for ColorBox -->
    <link   href="js/jquery.colorbox/colorbox.css" rel="stylesheet" type="text/css"/>
    <script src="js/jquery.colorbox/jquery.colorbox-min.js" type="text/javascript"></script>
    
    <!-- These files are the PWI files -->
    <link   href="css/pwi.css" rel="stylesheet" type="text/css"/>
    <script src="js/jquery.pwi-min.js" type="text/javascript"></script>

    <script type="text/javascript">

      $(document).ready(function () {
        var settings = {
            username: 'tester',  <!-- REPLACE WITH YOUR PICASA NAME!!!! -->
            colorbox_config: {
                config_photos: {
                    loop: true
                },
                config_youtube: {
                    innerWidth: '50%',
                    innerHeight: '50%',
                }
          };
        $("#container").pwi(settings);
      });

    </script>

```

Here the loop-option for photos is switched on and for YouTube videos the width and height is reduced to 50 percent.

Within colorbox\_config 4 different configuration sections are defined:

| Name | Description |
|:-----|:------------|
| config\_photos | Configuration options used when viewing photos |
| config\_youtube | Configuration options used when viewing YouTube videos |
| config\_maps | Configuration options for photo-maps. This is the map shown for one photo |
| config\_map\_overview | Configuration options for the overview map |

Within these sections specific configuration options can be set for Colorbox. These options will be used when showing specific item. For example, the default for photos is to show navigation (previous/next), for YouTube videos this is disabled.

See http://jacklmoore.com/colorbox/ for more information on Colorbox and on the other configuration options.

# Demos #

All demos include a Colorbox demo, but there are also some demos available in this Wiki:
  * Go to [here](ColorBoxDemoLatest.md) for a demo using the latest and greatest version of PWI
  * Go to [here](ColorBoxDemoCurrent.md) for a demo using the latest released version of PWI
