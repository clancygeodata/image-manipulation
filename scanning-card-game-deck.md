# Scanning Playing Cards

One of my favorite card games is [Parade](https://boardgamegeek.com/boardgame/56692/parade). It is a game for 2 to 6 players that lasts around half an hour per game. If you're curious about how to play, check out [the game rules](https://github.com/clancygeodata/image-manipulation/blob/master/zm1201_parade_rules.pdf).

I have been playing card games online with some friends by using [playingcards.io](https://playingcards.io/), a simple, convenient, and free website for creating a virtual table for a card game. Some of its features include automated card recalling, shuffling, and dealing. Customizable decks of cards can be used by adding text or images to the virtual cards. I wanted images to use for a virtual deck of cards for Parade, so I scanned each card.

## Scanning each card

To have consistent orientation of the cards and simplify the cropping process later, I individually scanned each card aligned in the top right corner of the scanning extent. I used the flatbed scanner of an HP OfficeJet Pro 9015. I used the HP Smart software to control the scanner and save the images. I scanned the cards at a resolution of 600 dpi. Here is one of the resulting images, after being cropped to fit the illustration on the card:

![alt text](https://github.com/clancygeodata/image-manipulation/blob/master/purple_2_scan.jpg)

The initial images are relatively high resolution for my needs, but I wanted to scan at a high resolution and then scale them down lower to be used for the virtual cards. Here is the same image, but scaled down to a resolution suitable for use in the virtual card table (via [playingcards.io](https://playingcards.io/)):

![alt text](https://github.com/clancygeodata/image-manipulation/blob/master/purple_2_scan_low_res.jpg)

The images look okay at this point, but the grid of the screened card surface is prominantly visible. I would rather it be less visible, but how can that be accomplished?

## Improving the images

GIMP (GNU Image Manipulation Program)...
Several plugins for GIMP...

## G'MIC plugin for GIMP

Description of G'MIC
Link to GitHub
List functions I tried...

## Descreen filter in G'MIC

Applied this filter twice...
Description of the filter...
Link to GitHub

## Before vs after descreen

image vs image

## BIMP for GIMP

BIMP (Batch Image Manipulation Plugin) provides a convenient graphical user interface for applying the same tools, filters, manipulations, etc. to a group or batch of images.

## G'MIC within BIMP

Description...

<a href="http://www.youtube.com/watch?feature=player_embedded&v=DJh1AB0VdFk
" target="_blank"><img src="http://img.youtube.com/vi/DJh1AB0VdFk/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>
## Final color adjustments

