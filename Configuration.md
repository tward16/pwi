﻿#summary Configuring PWI

# Configuring PWI #

The following is an overview of all the options you can set.

## General Settings ##

| **Name** | **Default** | **Description** |
|:---------|:------------|:----------------|
| username | ""          | REQUIRED TO SET, NOT OPTIONAL, THE REST IS!!! |
| mode     | 'albums'    |  can be: album, albums, latest |
| album    | ""          |  specify an album name if mode is 'album' (see name in URL of Picasa Web interface for correct album name) |
| authKey  | ""          |  specify the authKey if you choose mode 'album' and specified an unlisted album from picasa |
| keyword  | ""          | Filter photos based on keywords. See [Filtering albums and Photos](Filtering.md) for more information |
| showPager | 'bottom'    | 'top', 'bottom', 'both' (for both albums and album paging) |
| useQueryParameters | true        | Allow use of query parameters in the URL (parameters after a question-mark), to pass parameters to PWI. Needed for perma-link feature. [See below](#Query_parameters.md) |
| loadingImage | ""          | This image will be shown when data is being requested from Picasa |
| labels   |             | [See below](#Labels.md) |
| months   |             | [See below](#Months.md) |
| fancybox\_config | { }         | See [Fancybox](Fancybox.md) page for configuration options |
| colorbox\_config | { }         | See [Colorbox](Colorbox.md) page for configuration options |
| slimbox\_config | { }         | See [Slimbox](Slimbox.md) page for configuration options |
| blockUIConfig | { }         | See http://malsup.com/jquery/block/#options for configuration options. |

## Setting for Album overview ##

| **Name** | **Default** | **Description** |
|:---------|:------------|:----------------|
| albums   | [.md](.md)  |  specify a list of album names if mode is 'albums', leave as [.md](.md) to show all albums (ex. ['album1','album2'])  |
| albumTypes | "public"    |  currently not supported: "private", "all", "visible" |
| albumCrop | 1           |  crop the thumbs of the albums (1 = yes / 0 = no) |
| albumKeywords | ""          | Filter albums based on keywords. See [Filtering albums and Photos for more information](Filtering.md) |
| albumMaxResults | 999         |  display maximum number of albums |
| albumPage | 1           |  force load on specific album |
| albumsPerPage | 999         |  show X albums per page (activates paging on albums when this amount is less then the available albums) |
| albumTitle | ""          |  displays alternative album title if no title is specified in Picasa |
| albumThumbAlign | 1           | Allign thumbs vertically between rows |
| albumThumbSize | 72          |  specify thumbnail size of albums (supported cropped/uncropped: 32, 48, 64, 72, 104, 144, 150, 160 and uncropped only: 94, 110, 128, 200, 220, 288, 320, 400, 512, 576, 640, 720, 800, 912, 1024, 1152, 1280, 1440, 1600)) |
| albumStartDateTime | ""          | Albums on or after this date will be shown. See [Filtering albums and Photos for more information](Filtering.md) |
| albumEndDateTime | ""          | Albums before or on this date will be shown.See [Filtering albums and Photos for more information](Filtering.md) |
| onclickAlbumThumb | ""          |  overload the function when clicked on a album thumbnail |
| removeAlbums | ""          | Remove specific album from overview |
| removeAlbumTypes | ""          | Albums with this type in the gphoto$albumType will not be shown. Known types are Blogger, ScrapBook, ProfilePhotos, Buzz, CameraSync |
| showAlbumdate | true        |  Display date underneath album thumbs |
| showAlbumDescription | true        |  Display album description on photo page |
| showAlbumLocation | true        |  Display location (if specified) of album in album description on photo page |
| showAlbumPhotoCount | true        |  Display amount of photo's in album underneath album thumb |
| showAlbumTitles | true        |  Display title underneath album thumbs |
| showAlbumTitlesLength | 9999        | Maximum length of an album title to show |
| showAlbumThumbs | true        | Show albums as thumbs on albums overview page |
| sortAlbums | "none"      |  Sort the albums, allowed values: none, ASC\_DATE, DESC\_DATE, ASC\_NAME, DESC\_NAME |

## Setting for Photo overview ##

| **Name** | **Default** | **Description** |
|:---------|:------------|:----------------|
| page     | 1           |  Set to page if mode is 'album' and you want to start at a certain page of the album when the page is loaded. |
| photoSize | auto        |  Photo size to link to in the album (supported: auto, 94, 110, 128, 200, 220, 288, 320, 400, 512, 576, 640, 720, 800, 912, 1024, 1152, 1280, 1440, 1600) |
| maxResults | 50          |  Maximum amount of photo's per album page |
| thumbSize | 72          |  specify thumbnail size of photo's (supported cropped/uncropped: 32, 48, 64, 72, 104, 144, 150, 160 and uncropped only: 94, 110, 128, 200, 220, 288, 320, 400, 512, 576, 640, 720, 800, 912, 1024, 1152, 1280, 1440, 1600)  |
| thumbCrop | false       |  crop the thumb of the photo's (1 = yes / 0 = no) cropping makes the thumbs square and gives consistent layout |
| thumbAlign | false       | Allign thumbs vertically between rows |
| thumbCss | {'margin':'5px'} | override and add custom styles for the thumbs (see http://docs.jquery.com/CSS/css#properties for specification) |
| onclickThumb | ""          |  override click on single photo thumb. specify a function to replace slimbox,see demo 3 for an example |
| showPhotoCaption | false       |  Show caption underneath photo thumb (not recommended to prevent layout issues) |
| showPhotoCaptionDate | false       | Show photo date in caption |
| showCaptionLength | 9999        | Maximum length of a photo caption to show |
| showPhotoDownload | false       | Show download link next to each photo on album page |
| showPhotoDownloadPopup | false       | Show download link next to photo description on the photo popup in Slimbox and Fancybox |
| showPhotoDate | true        |  Show photo date in caption |
| showPermaLink | false       | Show a perma-link box at the bottom of an album page, containing a link to the current page |
| showPhotoLocation | false       | Process geo-information of a picture, showing on Google maps when data is available |
| mapIconLocation | ""          | Icon that will be shown when location information is available for a picture |
| mapSize  | 0.75        | Size of the map, relative to the size of browserwindow |
| sortPhotos | "none"      |  Sort the albums, allowed values: none, ASC\_DATE, DESC\_DATE, ASC\_NAME, DESC\_NAME |
| videoBorder | "images/video.jpg" | Image that will be used to overlap the thumbnail of a video |

## Labels ##

To translate the labels fill in the labels with texts in your language, or just with different texts. The following texts can be translated:

| **Label** | **Default** |
|:----------|:------------|
| photo     | photo       |
| photos    | photos      |
| downloadphotos | Download photos |
| albums    | Back to albums |
| noalbums  | No albums available |
| page      | Page        |
| prev      | Previous    |
| next      | Next        |
| showPermaLink | Show PermaLink |
| showMap   | Show Map    |
| videoNotSupported | Video not supported |

See [Example](#Example.md) below on how to add these to your configuration.

## Months ##

To translate the monthnames fill in the names with the names in your language.

## Query parameters ##

Query parameters are used to pass information to a web page using the URL. This is the information usually after a question mark. PWI supports the following query parameters:

| **Parameter** | **Description** |
|:--------------|:----------------|
| pwi\_album\_selected | Album to be selected. Changes mode to album. |
| pwi\_albumpage | Page within an album to show. Should be less than the number of pages in an album. Note that when the setting maxResults is changed this value should also be changed. |
| pwi\_showpermalink | Overrules the showPermaLink setting, showing the perma-link box at the bottom of the page. Can be used to request a perma-link of a page without modifying the settings |

An example of a URL containg these query parameters:

http://pwi.googlecode.com/svn/tags/REL_2_0_0/demo9.html?pwi_album_selected=DanceParade2008&pwi_albumpage=4

Note that the permalink feature will be switched off when a specific page is selected using this feature.

## Example ##

Below is an example on how to change certain settings and labels of PWI. Make sure you end each setting with a comma except for the last one.

```
$(document).ready(function() {

	var options = {
		username: 'YourPicasaUserName',
		mode: 'albums',
		albums: ["Album1","Album2"],
		labels: {photo:"picture",
		         photos: "pictures"
		        },
        months: ["JANUARY", "FEBRUARY", "MARCH", "APRIL", "MAY", "JUNE", "JULY", "AUGUST", "SEPTEMBER", "OCTOBER", "NOVEMBER", "DECEMBER"],
	};

	$("#container").pwi(options);

});
   
```

This example will show the albums page with thumbnails of Album1 and Album2 of Picasa user YourPicasaUserName. Instead of the label "photo" the label "picture" will be used. All month names will be in capitals.