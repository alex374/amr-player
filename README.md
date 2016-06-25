amr-player
play remote amr format audio with JavaScript

inpired by https://github.com/yxl/opencore-amr-js

-- AmrPlayer --
params:
  amr_url
  download_success_cb (optional)
  download_progress_cb (optional)
props:
  bool canPlay
  bool isPlaying
methods:
  play()
  pause()
  toggle() // play() when paused or pause() when playing
  endWith(callback) // optional, fire callback with ended event

usage:
    <script src="xxx/amrnb.js"></script>
    <script src="xxx/amrplayer.js"></script>
	  
	var player = new AmrPlayer('http://xxx.com/xxx.amr');
	player.endWith(function(){ console.log( xxx ) });
	player.play();
	// player.pause();
	// player.toggle();
