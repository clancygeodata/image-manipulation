# Scanning Playing Cards

One of my favorite card games is [Parade](https://boardgamegeek.com/boardgame/56692/parade). It is a game for 2 to 6 players that lasts around half an hour per game. If you're curious about how to play, check out [the game rules](https://github.com/clancygeodata/image-manipulation/blob/master/zm1201_parade_rules.pdf).

I have been playing card games online with some friends by using [PlayingCards.io](https://playingcards.io/), a simple, convenient, and free website for creating a virtual table for a card game. Some of its features include automated card recalling, shuffling, and dealing. Customizable decks of cards can be used by adding text or images to the virtual cards. I wanted images to use for a virtual deck of cards for Parade, so I scanned each card.

## Scanning each card

To have consistent orientation of the cards and simplify the cropping process later, I individually scanned each card aligned in the top right corner of the scanning extent. I used the flatbed scanner of an HP OfficeJet Pro 9015. I used the HP Smart software to control the scanner and save the images. I scanned the cards at a resolution of 600 dpi. Here is one of the resulting images, after being cropped to fit the illustration on the card:

![alt text](https://github.com/clancygeodata/image-manipulation/blob/master/purple_2_scan.jpg)

The initial images are relatively high resolution for my needs, but I wanted to scan at a high resolution and then scale them down lower to be used for the virtual cards. Here is the same image, but scaled down to a resolution suitable for use in the virtual card table (via [PlayingCards.io](https://playingcards.io/)):

![alt text](https://github.com/clancygeodata/image-manipulation/blob/master/purple_2_scan_small.jpg)

The images look okay at this point, but the screened texture on the card surface is prominantly visible as a grid of dots. I would rather it be less visible, but how can that be accomplished?

## Improving the images

To crop and scale down the images, I used [GIMP](https://www.gimp.org/) (GNU Image Manipulation Program), which is free and open source image editing software (similar to Adobe Photoshop, but free). GIMP has many options for enhancing and modifying images. A variety of plugins can be added in GIMP for even more options.

## G'MIC-Qt plugin for GIMP

[G'MIC](https://gmic.eu/) is an open source collection of image manipulation tools with multiple options for user interfaces. [G'MIC-Qt](https://github.com/c-koi/gmic-qt) is a plugin that provides G'MIC with a user interface for GIMP and other image software (Krita, Photoshop, Affinity Photo, PaintShop Pro, PhotoLine, and Paint.NET).

G'MIC has many powerful image filters. Here are some of the G'MIC filters that I tried using for making the dot grid less visible in the images or isolating it:
- Frequencies > Fourier Transform
- Details > Split Details [Gaussian]
- Details > Split Details [Wavelets]
- Repair > Unstrip
- Repair > Despeckle
- Repair > Smooth [Median]
- Repair > Descreen

## Descreen filter in G'MIC

![alt text](https://github.com/clancygeodata/image-manipulation/blob/master/purple_2_descreen.jpg)

Applied this filter twice...
Description of the filter...
Link to GitHub

## Before vs after

![alt text](https://github.com/clancygeodata/image-manipulation/blob/master/purple_2_scan_small.jpg)![alt text](https://github.com/clancygeodata/image-manipulation/blob/master/purple_2_descreen_small.jpg)

## BIMP for GIMP

BIMP (Batch Image Manipulation Plugin) provides a convenient graphical user interface for applying the same manipulation processes to a group or batch of images. Once I chose the processes I wanted to use for one image, I used BIMP to conveniently apply those processes to all of the card images.

## G'MIC within BIMP

This video demonstrates how to use G'MIC filters

<a href="http://www.youtube.com/watch?feature=player_embedded&v=DJh1AB0VdFk
" target="_blank"><img src="http://img.youtube.com/vi/DJh1AB0VdFk/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>
## Color adjustments

Some of the images were too brightly colored, especially those of the yellow cards. I made some color adjustments to make them easier to read.