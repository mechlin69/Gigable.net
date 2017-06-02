---
ID: 7666
post_title: Streamsong
author: Mike Echlin
post_date: 2017-05-26 18:46:57
post_excerpt: ""
layout: page
permalink: https://www.gigable.net/streamsong/
published: true
---
<audio controls>
  <source src="song">
Your browser does not support the audio element.
</audio>

<script type="text/javascript">
var queryString= window.location.search;
queryString = queryString.substring(51);
var tune = queryString.slice (0, -4);
var songUrl = audio("https://s3-us-west-2.amazonaws.com/gigable.tracks/" + tune + ".mp3");
document.getElementById("song").innerHTML = "songUrl";
</script>