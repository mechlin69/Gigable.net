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
<script type="text/javascript">
var queryString= window.location.search;
queryString = queryString.substring(51);
var tune = queryString.slice (0, -4);
var song = "https://s3-us-west-2.amazonaws.com/gigable.tracks/" + tune + ".mp3";
document.write(song);
$("a").click(function() {
  $("song").play();
});

$(document).ready(function(){
$("#jquery_jplayer_1").jPlayer({
ready: function () {
$(this).jPlayer("setMedia", {
mp3: "song",
oga: "/media/mysound.ogg"
});
},
swfPath: "/js",
supplied: "mp3, oga"
});
});
</script>
<div id="jquery_jplayer_1"></div>
<div id="jp_container_1">
<a href="#" class="jp-play">Play</a>
<a href="#" class="jp-pause">Pause</a>
</div>