#MediaElement-Markers - Markers on the Progress bar

![MediaElement marker](https://raw.github.com/sourcebits-harshitakasera/mediaelement-markers/master/markers.png "Marker")

__Author__   - Harshita Kasera  
__License__   - GPLv2/MIT 


# Introduction

MediaElement-Markers is a <code>MediaElement.js</code> plugin that lets you add ___Visual Cues___ in the progress time rail. This plugin also lets you register a custom callback function that will be called everytime the play position reaches a marker. Marker position and a reference to the MediaElement Player object is passed to the registered callback function for any post processing. Marker color is configurable. 

# Demo
[Click here](http://jsfiddle.net/hkasera/a3dBe/4/) to see a working demo of the plugin.
# Credits

My Employer - [Sourcebits Inc.](http://www.sourcebits.com)

Thanks to [John Dyer](https://github.com/johndyer), creator of [MediaElement Player](http://mediaelementjs.com/)

# Installation & Usage

### Installation
    <script src="jquery.js"></script>
    <script src="mediaelement-and-player.min.js"></script>
    <script src="mep-feature-markers.js"></script>
    <link rel="stylesheet" href="mediaelementplayer.css" />

### Usage
    $('#player').mediaelementplayer({
        features: ['playpause','current','progress','duration','markers'], //Adding the feature 'markers' enables this plugin
        markerColor: '#FCD730', // Optional : Specify the color of the marker
        markers:['4','16','20','25','35','40'], // Specify marker times in seconds 
        markerCallback:function(media,time){ // Callback function invoked when a marker position is reached
           /* Your Code */
        }
    });

# Testing
    *IE7 - Flash 
    *IE8 - Flash
    IE9, IE10 - MP4
    Firefox - Ogv
    Chrome - Webm
    Safari - MP4
    
<code>* Note</code> Markers will appear only after Play in IE7 and IE8 due to the limitation in Flash Player.

# Version History

*1.0.0 (2013/01/14)*    
&nbsp;&nbsp;&nbsp;Initial release
