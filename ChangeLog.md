﻿#summary PWI Change Log.
#labels Featured

### Latest ###

  * FIXES:
    * [Issue 105](https://code.google.com/p/pwi/issues/detail?id=105) (bug): Make sure PWI does not use settings from other PWI instance
    * [Issue 106](https://code.google.com/p/pwi/issues/detail?id=106) (bug): Make sure you cannot navigate from one PWI instance to another

### Updates v2.0 ###

  * NEW:
    * Upgrade to jQuery 1.7.1.
    * Upgrade to FancyBox 2.0
    * Added ColorBox support
    * Redesign of demos: allow user to choose which viewer to use
    * Added support for YouTube videos from Picasa
    * Sorting of albums and photos, using name or date (ascending and descending)
    * Select maximum size of photo that can displayed
    * Improved overview of albums and album layout
    * Improved paging of selection of albums
    * [Issue 43](https://code.google.com/p/pwi/issues/detail?id=43) (feature request): Added option to show map of a picture: for each photo separate and an overview map of all photos in an album
    * [Issue 76](https://code.google.com/p/pwi/issues/detail?id=76) (feature request): Leave albums displayed while viewing pictures: updated demo8 (now demo5)
    * [Issue 87](https://code.google.com/p/pwi/issues/detail?id=87) (feature request): Option to exclude specific albums
  * FIXES:
    * [Issue 68](https://code.google.com/p/pwi/issues/detail?id=68) (bug): Upgraded blockui to 2.39
    * [Issue 83](https://code.google.com/p/pwi/issues/detail?id=83) (bug): Issue with user@company.com
    * [Issue 86](https://code.google.com/p/pwi/issues/detail?id=86) (bug): Documentation update
    * [Issue 89](https://code.google.com/p/pwi/issues/detail?id=89) (bug): Translating labels could break PWI
    * [Issue 90](https://code.google.com/p/pwi/issues/detail?id=90) (bug): Albums pagination
    * [Issue 95](https://code.google.com/p/pwi/issues/detail?id=95) (bug): Photo description missing

### Updates v1.5 ###

  * NEW:
    * Added Permalink feature using Query parameters
    * Improved download link function, including extra option to control this
    * Optionally remove albums with type Blogger, Scrapbook and/or ProfilePhotos albums

  * FIXES:
    * Fixed alignment on albums overview page
    * [Issue 82](https://code.google.com/p/pwi/issues/detail?id=82): fixed issue with dots in Picasa account name
    * Fixed showPhotoDownload handling

### Updates v1.4.1 ###

  * FIXES:
    * Reset some defaults back to the 1.3 values
    * Fixed an issue where the albums overview would use the album thumbs settings

### Updates v1.4 ###

  * NEW:
    * Added Download link to picture.
    * Implemented slideshow in Fancybox
    * Added more filtering options for albums view (date + keyword)
    * Upgrade to jQuery 1.6.2 and Fancybox 1.3.4

  * FIXES:
    * Photo navigation not limited to thumbs shown, but all photos from the album can be seen
    * Optimized Picasa/Google API requests
    * some minor issues

### Updates v1.3 ###

  * NEW:
    * Album paginating
    * onClickThumb and onClickAlbum return full data stream for you to use (advanced)
    * Short captions on thumbs, long in Photo popup
    * Show album titles only (in demo 11)
    * use keywords in any mode

  * FIXES:
    * cropping issues resolved
    * JSLINT validation
    * Line breaks in photodescription
    * some minor issues


### New features (v1.2): ###

  * optional dependencies of jQuery BlockUI and slimbox2 plugin
  * 4 different modes:
    * album  (single album view)
    * albums (all or specific albums)
    * keyword (photo's from all albums with specific keyword) (**new in v1.2**)
    * latest (showing the last photo's uploaded)
  * multiple modes on 1 page
  * add custom popup plugins like fancybox
  * compatible with jQuery 1.4
  * and much more... will follow soon.