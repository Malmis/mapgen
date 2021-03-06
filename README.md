mapgen
======

Script to make your own OpenStreetMap maps for Garmin GPS units.

Right now the script uses mostly Swedish language, but maybe sometime it will be translated to English.

This script uses and downloads pre-generated *.osm.pbf files from geofabrik.de.


### HOW TO ###

Before your run the script, you may take a look inside it and change some stuff, i.e. the name of country you would like to map a map for.

You run it with:

    ./mapgen

it will output a help menu with every command you could use.

The output of ./mapgen will be:

    $ ./mapgen
    Dessa kan du använda:
    -i eller install (Behöver bara köras första gången.)
    -d eller download (Laddar ner OSM data för Sweden.)
    -s eller split (Splittar och förbereder filer.)
    -k eller kust (Laddar ner kustlinjer för din karta. Behöver bara köras en gång.)
    -b eller build (Genererar standardkarta.)
    -p eller polygon (Laddar ner polygon för Sweden. Behöver bara köras en gång per land.)
    -pbf eller pbf-files (Genererar pbf-filer för topografiska linjer.)
    -img eller image-files (Genererar image filer för topografisk karta.)
    -me eller merge (Slår ihop standardkartan med topografiska linjer.)
    -cp eller copy (Kopierar standardkarta till /home/osm/public_html/garmin/.)
    -cp2 eller copy2 (Kopierar karta med topografiska linjer till /home/osm/public_html/garmin/.)
    -m eller move (Flyttar standardkarta till /home/osm/public_html/garmin/.)
    -m2 eller move2 (Flyttar karta med topografiska linjer till /home/osm/public_html/garmin/.)
    -c eller clean (Rensar bort alla filer för Sweden så att inte gamla filer ska ligga kvar nästa gång du vill skapa en ny karta.)


### Functions ###
The script is not completely done yet, so there are some missing functions in it right now.

But right now i have implemented this stuff:
* Complete one command installation (creates necessary directories and downloads styles and tools).
* Download of country *.osm.pbf files from geofabrik.
* Automated splitting of country file.
* Creation of new args file.
* Downloads coastlines with one command.
* Builds maps ready to use in Garmin GPS units.
* Downloads srtm3 (topographic) data and creates pbf files of them.
* Builds garmin image files of the topographic data.
* Download polygon file.
* Merging of standard map and topographic map.
* Move function to move the ready garmin image files to wherever you want them to be.
* Cleaning function to remove unnecessary files after you have built your map completely.


### Help & Contact ###
If you need to contact me, you cand find me on IRC on freenode, dalnet, quakenet and oftc as Malmis.
You could also send me an email if you don't know how to use IRC.

Email: mitod1@gmail.com
