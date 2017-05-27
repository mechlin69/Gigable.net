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
<script>
var queryString= window.location.search;
queryString = queryString.substring(51);
var tune = queryString.slice (0, -4);
var song = "https://s3-us-west-2.amazonaws.com/gigable.tracks/" + tune + ".mp3";
document.write(song);
$("a").click(function() {
  $("audio").play();
});
</script>