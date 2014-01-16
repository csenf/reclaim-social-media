Reclaim Social Media
====================

Reclaim Social Media version .2, based on Reclaim Social Media version .1 by
[Felix Schwenzel](http://reclaim.fm) & Sascha Lobo.

It’s a single Wordpress plugin by remigi illi at [digitaleheimat.de](http://digitaleheimat.de), instead of a collection of proxy-scripts and 3rd party plugins. The code of the early version can be found at GitHub ([proxy scripts](https://github.com/diplix/reclaim-proxy-scripts)) and the [reclaim.fm site](http://reclaim.fm/tech-specs-details/).

The plugin is still pretty raw but should be a good foundation for further development.

## What it does
Right now reclaim grabs your tweets, Google+ and Facebook posts, Flickr and Instagram images, YouTube and Vine videos and imports them as Wordpress posts. It is written in a modular fashion, which enables anyone to easily write further importer modules for other services.

If reclaim grabs a tweet, it constructs an embed code with clickable hashtags, mentions and real links (unshortened t.co links). To do that, you need to get an API key from Twitter. This is a little complicated, but very much on purpose. We don't want to create a central application, that can be shut down at will by Twitter, but instead many decentralized apps with individual API keys, that can not be shut down easily.

The Twitter embed code is being rendered with Twitter's widget.js, which is a little invasive on users privacy, but looks nice. Also, the embed-code is fully searchable within Wordpress. In case an image is attached, it is being saved in the Wordpress media library and set as the featured image. Note that with some themes this may cause the image to be shown twice.

The idea is to copy all the relevant data from the services you use and to enable you to keep a copy on your own server.

## Demo
http://root.wirres.net/reclaim/

## Installation
Download a [release](https://github.com/espresto/reclaim-social-media/releases) or clone the repository. If you clone, don't forget to run composer. Also remember, the plugin is not stable yet.
