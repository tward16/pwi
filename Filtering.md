﻿#summary Filtering

# Introduction #

When using the Albums nomally all albums are shown. Using the methods described
on this page it is possible to selecte a subset of the albums. This can for
example be used to show only the albums of a certain year.

# Filtering Albums #

The albums shown can be filtered using three methods: on album name, on date and
on keywords.

  * Album name: using the albums-setting it is possible to select a subset of albmums using the names as given by Picasa.
  * Date: using the albumStartDateTime and albumEndDateTime it is possible to select a certain period. See Demo 8 for an example.
  * AlbumKeywords: the keywords given in this setting are matched against keywords given in the description of the album. If all keywords match the album is shown in the overview. The keywords should be specified in the Picasa album description using:

```
    [keywords: "keyword1", "keyword2"]
```

# Filtering Photos #

It is possible to filter photo's from different albums using keywords, see Demo 3.

The photo's within an album can be filtered using the keyword-setting.
