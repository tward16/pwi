﻿#summary PWI: Using SlimBox2

# Using SlimBox2 #

One of the ways to show the photo's is by using Slimbox (http://www.digitalia.be/software/slimbox2). PWI includes an unmodified version of the Slimbox2 scripts.

To use the Slimbox script the Slimbox JavaScript library needs to loaded.  Use the following code in the header of your
page to load PWI with Slimbox support:

```

    <!-- This can be your local jquery lib, but why not have it hosted by Google -->
    <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.7.2/jquery.min.js"></script>

    <!-- These files are needed for SlimBox -->
    <link   href="js/jquery.slimbox2/jquery.slimbox2.css" rel="stylesheet" type="text/css"/>
    <script src="js/jquery.slimbox2/jquery.slimbox2.js" type="text/javascript"></script>

    <!-- These files are the PWI files -->
    <link href="css/pwi.css" rel="stylesheet" type="text/css"/>
    <script src="js/jquery.pwi.js" type="text/javascript"></script>

    <script type="text/javascript">

      $(document).ready(function () {
        var settings = {
            username: 'tester'   <!-- REPLACE WITH YOUR PICASA NAME!!!! -->
          };
        $("#container").pwi(settings);
      });

    </script>

</script>

```

# Slimbox settings #

Configuring Slimbox can be done using the slimbox\_config setting, as indicated on the [Configuring PWI](Configuration.md) page. The slimbox\_config setting can contain the following settings:

| **Name** | **Default** |
|:---------|:------------|
| loop     | false       |
| overlayOpacity | 0.6         |
| overlayFadeDuration | 400         |
| resizeDuration | 400         |
| resizeEasing | "swing"     |
| initialWidth | 250         |
| initlaHeight | 250         |
| imageFadeDuration | 400         |
| captionAnimationDuration | 400         |
| counterText | "{x}/{y}"   |
| closeKeys | `[`27, 88, 67, 70`]` |
| prevKeys | `[`37, 80`]` |
| nextKeys | `[`39, 83`]` |


See the [Slimbox website](http://www.digitalia.be/software/slimbox2) for the exact meaning of these options.

# Example #

You can change any of theses settings by adding the new settings after the username setting. So, if you want to change the countertext you can do that using this code to replace the code in the first example:

```

    $(document).ready(function() {  //-- default jQuery call, do stuff when page is loaded
        $("#container").pwi({  //--specify your DIV's ID here
            username: 'tester',  //--REPLACE WITH YOUR PICASA NAME!!!!
            slimbox_config: {
                counterText: "Picture {x} of {y}"
            }
        });
    });

```

See http://www.digitalia.be/software/slimbox2 for more information on Slimbox and on the configuration options.

# Demos #

A number of demos are available in the distribution, but there are also some demos available in this Wiki:
  * Go to [here](SlimBoxDemoLatest.md) for a demo using the latest and greatest version of PWI
  * Go to [here](SlimBoxDemoCurrent.md) for a demo using the latest released version of PWI