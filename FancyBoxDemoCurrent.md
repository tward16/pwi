#summary FancyBox Demo

# Introduction #

On this page a number of demo's will be shown using the FancyBox jQuery plugin amd the current release of PWI,
showing a number of possibilities of the pwi application.

The following demo's are shown:
  * [Default usage](FancyBoxDemoCurrent#Demo_1:_Default_usage.md)
  * [Some extra layout options](FancyBoxDemoCurrent#Demo_2:_Some_extra_layout_options.md)
  * [Grouped by year](FancyBoxDemoCurrent#Demo_3:_Grouped_by_year.md)


# Demo 1: Default usage #

This demo shows the use of FancyBox without any configuration.

The following settings are used for this demo:
```
    var settings = {
        username: '<USERNAME>'
    }
    $("#container").pwi(settings);
```
&lt;wiki:gadget url="http://pwi.googlecode.com/svn/wiki/PwiGadget/FancyBox/FancyBoxDemo1\_Current.xml" width="640" height="480" /&gt;

# Demo 2: Some extra layout options #

This demo shows the use of FancyBox with a number of extra layout options:
  * Smaller uncropped album thumbnails
  * Cropped picture thumbnails
  * Download link in photo description in Fancybox popup
  * Show waiting-image when loading
  * Remove albums with type ScrapBook and ProfilePhoto
  * Show map when location is available (see Marathon Rotterdam map)

The following settings are used for this demo:
```
    var settings = {
        username: '<USERNAME>',
        showPhotoDownloadPopup: true,
        showPhotoCaption: true,
        showPhotoLocation: true,
        mapIconLocation: "images/icon-earth.png",
        albumCrop: 0,
        albumThumbSize: 72,
        thumbCrop: 1,
        thumbAlign: 1,
        removeAlbumTypes: ["ScrapBook", "ProfilePhotos"]
    }
    $("#container").pwi(settings);
```
&lt;wiki:gadget url="http://pwi.googlecode.com/svn/wiki/PwiGadget/FancyBox/FancyBoxDemo2\_Current.xml" width="640" height="480" /&gt;

# Demo 3: Grouped by year #

This demo shows the grouping per year. Each div in the HTML code shows only one year. For each div the start and end date are specified in the var section. For each div a special var section is needed.

The following settings are used for this demo:
```
    var settings2007 = {
        username: '<USERNAME>',
        albumStartDateTime: "2007-01-01", 
        albumEndDateTime: "2007-12-31"
    }
    var settings2008 = {
        username: '<USERNAME>',
        albumStartDateTime: "2008-01-01", 
        albumEndDateTime: "2008-12-31"
    }
    var settings2009 = {
        username: '<USERNAME>',
        albumStartDateTime: "2009-01-01", 
        albumEndDateTime: "2009-12-31"
    }
    
    $("#container2007").pwi(settings2007);
    $("#container2008").pwi(settings2008);
    $("#container2009").pwi(settings2009);
```
&lt;wiki:gadget url="http://pwi.googlecode.com/svn/wiki/PwiGadget/FancyBox/FancyBoxDemo3\_Current.xml" width="640" height="480" /&gt;