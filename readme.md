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
