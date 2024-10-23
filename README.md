This little program is made to quickly visualise clumps in Euclid tiles. It uses filters to detect a given angular scale of clumps, then shows the contours of the filtered image superposed on the tile part. The tiles must be downloaded in the Euclid_tiles folder.

SETTINGS :

The main code is euclid_image_test.py in the PROG folder. All modifications by the user are made in it.

-The name of the tile (not its path !) must be referenced in the string variable imagename
-The code offers to only work with a little part of the tile as they are usually quite big. The center RA (hms), dec (degrees) and angular radius (arcsec) of the tile part must be specified in euclid_image_test.py . RA and Dec must be given in hourangle and degrees respectively, in the astropy format (strings "..h..m..s" and "..d..m..s").
-The clump_angular_size variable is simply the angular size of the luminosity variations one wants to outline in the image

OTHER REMARKS

-The final image is shown in log scale.
-It is possible to take masks into account, mainly to remove stars from the field (this option is already implemented, I just need to make it easy to use).