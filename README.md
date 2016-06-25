amr-player
play remote amr format audio with JavaScript
inpired by https://github.com/yxl/opencore-amr-js

* -- AmrPlayer --
* params:
*  1. amr_url
*  2. download_success_cb (optional)
*  3. download_progress_cb (optional)
* props:
*  1. bool canPlay
*  2. bool isPlaying
* methods:
*  1. play()
*  2. pause()
*  3. toggle() // play() when paused or pause() when playing
*  3. endWith(callback) // fire callback with ended event

usage:
	<script src="xxx/amrnb.js"></script>
    <script src="xxx/amrplayer.js"></script>
	  
	var player = new AmrPlayer('http://xxx.com/xxx.amr');
	player.endWith(function(){ console.log( xxx ) });
	player.play();
	// player.pause();
	// player.toggle();
