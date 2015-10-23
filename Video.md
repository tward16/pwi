#summary Showing YouTube videos

# Introduction #

It is possible to link pictures in Picasa to certain YouTube videos. When you click on this picture the YouTube video will be shown instead of the photo.

Note: As SlimBox does only support pictures this feature is not available when using SlimBox.

<br>
<h1>Showing YouTube videos</h1>

Showing YouTube videos is very easy:<br>
<br>
<ul><li>Select a picture that you want to use to show the video.<br>
</li><li>Start the description of the photo with <code>"[youtube: &lt;youtube-id&gt;]"</code>.<br>
</li><li>Add any additional test to the description.</li></ul>

For example, to show the video that is available in the demo (see folder Test) use the<br>
following description:<br>
<pre><code>[youtube: hgadtxgXZ_k]Show YouTube video<br>
</code></pre>

You can find the YouTube-ID in the URL when you are watching a video. The URL used by YouTube looks like this:<br>
<pre><code>http://www.youtube.com/watch?v=&lt;youtube-id&gt;&amp;hd=1<br>
</code></pre>
You should use the part that you see after the <code>"v="</code> and before the next <code>"&amp;"</code> or the end of the URL.<br>
<br>
<br>
<h1>Configuration</h1>

There is one general option for YouTube videos:<br>
<br>
<table><thead><th> <b>Name</b> </th><th> <b>Default</b> </th><th> <b>Description</b> </th></thead><tbody>
<tr><td> videoBorder </td><td> "images/video.jpg" </td><td> Image that will be used to overlap the thumbnail of a video </td></tr></tbody></table>

<br>
<h1>Why not use Picasa video?</h1>

I also looked at Picasa video before I decided to use YouTube instead. Why did<br>
I choose YouTube over Picasa?<br>
<br>
<ul><li>The Picasa video functionality is basically uploading and viewing, while YouTube offers many more features<br>
</li><li>To show the Picasa video takes much more effort than showing the YouTube video<br>
</li><li>Easier to show other video's, next to video's in your own account