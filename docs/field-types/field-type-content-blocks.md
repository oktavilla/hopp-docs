---
group: "field-type"
layout: default
title:  "Content Blocks Field"
parent: "Field Types"
---

# Content Blocks Field
{: .no_toc }

1. TOC
{:toc}

----------

## Paragraph Block

A text paragraph.
Allows only basic formatting like **bold**, *Italic* and [links](http://oktavilla.se).
Probably a customized Gutenberg block.

----

## Heading Block

A sub heading. Can be on levels h2-h4.
Probably a standard Gutenberg block.

----

## List Block

A list can either be bulleted or numbered. List items may contain basic formatting like **bold**, *Italic* and [links](http://oktavilla.se).
Probably a customized Gutenberg block.

----

## Image Block

Probably a custom block.

* [Image](field-type-image.md)
* Caption (defaults to the image asset caption, but can be overwritten)
* Visual Preference (one of `discreet`, `standard`, `prominent`)

----

## Gallery Block

Probably a custom block.
A group of images where each image has:

* [Image](field-type-image.md)
* Caption (defaults to the image asset caption, but can be overwritten)

----

## Separator

A divider for creating segements on a page. Probably a standard Gutenberg block.

----

## Fact Block

Probably a custom block.

* Title
* Paragraph Block(s)
* List Block(s)

----

## Quote Block

Probably a customized Gutenberg block.

* Paragraph Block(s)
* Source
* [Image](field-type-image.md)
* Visual Preference (one of `standard`, `prominent`)

----

## Teaser Block

A reference to a Content Item.
Probably a custom block.

----

## Embed Block

Probably a customized Gutenberg block.
Embed blocks makes in possible to insert third-party content (video, audio, images, tweets, etc.) from
trusted sources. It's possible to embed content from these sites:

* YouTube
* Twitter
* Facebook
* Instagram
* Vimeo
* Soundcloud
* Spotify
* Flickr
* Polldaddy

... and a few more.

----

## Map Position Block

Probably a custom block.
This is a block that can define a geographical position. It is basically just a bounding box comprised of:

* NE Coordinate (expressed as LatLng)
* SW Coordinate (expressed as LatLng)

And as another attribute:

* Caption
