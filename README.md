# Fonts

A selection of free and/or libre fonts. Liable to change.

Not found on Google Fonts at time of commit.

Each font or font family has its own directory, including license information.

Specimen waterfalls are provided.

## How It's Made

* Note: This is just a bunch of notes for me for when I'm having a wonky brain day. If you just want the font files, downlad the .zip and go nuts -- but remember to check the relevant license(s) to see what you're allowed to do with them. Caveat emptor.

You will need:

* A computer running macOS in some fashion, and the following tools:
 * Font Book (Finder -> Applications -> Utilities)
 * XnConvert
 * ImageOptim
* A heap of patience if your computer is a) one of mine, or; b) as slow as one of mine.
* ~1 gigabyte of free drive space for a full regeneration of waterfalls.

Let us begin.

## Adding font(s)

This is the easy part, and is relatively brisk:

* Check the license permits intended use, including redistribution.
* Check the font files are not available on Google Fonts.
* Obtain current release or latest build of said font as an archive.
* Preview the font(s) -- do they still look good? Were the designers sneaksy with their fancy previews?
* Install font(s) via Font Book, in the User Fonts folder. We don't need to vandalise the file system with our new and/or precious things.
* Drag new font(s) to `petecooper-fonts` collection. This naming is optional if you're not me. You do you, OK?

## (Re)generating font waterfall(s)

This part is still quite easy, but patience is needed.

* Turn off cloud, network and local backups since we're battering the desktop with some large files and this isn't a fast process.
* Select the font(s) in `petecooper-fonts` collection, ideally just the new ones but if you're feeling particularly sadistic you can select them all.
* Cmd+P to open the print dialog, then follow the settings as laid out in the `/tools/waterfall pdf output settings.png` file.
* Drop the created PDF onto `/tools/fonts waterfall pdf to png then xnconvert.app`, then allow some time for the PDF to make a lot of PNGs.
  * Optional step: do literally anything while this is underway, it can take many minutes.
* While this PDF to PNG magic is munching your CPU time, open XnConvert and apply the settings file from `/tools/xnconvert for waterfall png.xbs` using the XnConvert Actions panel and the diskette icon.
* When you have notification that the PDF to PNG stuff is complete, XnConvert will load the created PNGs into its input bin.
* Use the Convert button in XnConvert to make PNGs. They will overwrite the originals on the desktop.
  * Optional step: do literally anything while this is underway, it can take many more minutes than the previous thing that took many minutes.
* While XnConvert is chewing through its workload, open ImageOptim and apply the settings as shown in `/tools/imageoptim settings - general.png`, `/tools/imageoptim settings - quality.png` & `/tools/imageoptim settings - optimisation level.png`.
  * Yes, I'm using Insane optimisation on PNGs that XnConvert exported with zero compression. Fite me.
* Drag the XnConvert'd PNGs into ImageOptim and even more minutes than the previous thing that was already quite a lot of minutes.
  * This will seem like a week, but isn't. Consider doing the job you've been putting off for a while, it'll feel good when it's done.
* Consider using the Again button on the lower right of the ImageOptim window, especially if you're still doing the thing you kept putting off.
* Rename the PNGs to something sensible and drop into the respective waterfall directory.
  * Accept that you spending time and compute cycles squeezing bytes from files is for the greater good, and the internet tubes will be less busy as a result. Yay.
* Clear desktop of any detritus, and turn backups on again.

That's it. Thanks for playing.
