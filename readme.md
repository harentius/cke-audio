# Ckeditor html5 audio plugin

## Installation
### 1. Copy plugin to your project in any convenient way

Using [composer asset plugin](https://github.com/francoispluchino/composer-asset-plugin):

composer.json:

    "extra": {
    // ...
		"asset-repositories": [
			// ...
			{
				"type": "bower-vcs",
				"url": "git@github.com:harentius/cke-audio.git",
				"name": "bower-asset/ckeditor-audio-plugin"
			}
		]
    }

composer require bower-asset/ckeditor-audio-plugin


### 2. Configure Ckeditor

	CKEDITOR.plugins.addExternal("audio", "assets/vendor/ckeditor-audio-plugin/audio/plugin.js");

(or other installation path)

Inside config:

	extraPlugins: "...,audio"
## About
This is only an adaptation of Video plugin for CKEditor created by Alfonso Martínez de Lizarrondo

Originally forked from [https://github.com/Philalawst/cke_audio](https://github.com/Philalawst/cke_audio)

###List of improvements

#####by [aemr3](https://github.com/aemr3/cke_audio)
- Added autoplay/loop/controls options
- Changed default audio formats to mp3/wav
- Removed div around audio tags. (Causes some trouble)

#####by [harentius](https://github.com/harentius/cke-audio-plugin)
- Added plugin button to 'insert' group, stylized for Ckeditor 4
- Removed redundant second upload field
- Improved this readme
- Added file upload tab
