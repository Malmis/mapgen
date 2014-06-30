mapgen
======

Script to make your own OpenStreetMap maps for Garmin GPS units.

Right now the script uses mostly Swedish language, but maybe sometime it will be translated to English.

This script uses and downloads pre-generated *.osm.pbf files from geofabrik.de.


### HOW TO ###
When the script is downloaded, you need to make it executable with: 

    chmod +x mapgen


Before your run the script, you may take a look inside it and change some stuff, i.e. the name of country you would like to map a map for.


You run it with:

    ./mapgen

it will output a help menu with every command you could use.

The output of ./mapgen will be:

    $ ./mapgen
    Dessa kan du använda:
    -i eller install (Behöver bara köras första gången.)
    -d eller download (Laddar ner OSM data för Denmark.)
    -s eller split (Splittar och förbereder filer.)
    -a eller args (Skapar lista över alla filer som ska slås ihop.)
    -b eller build (Genererar standardkarta.)
    -pbf eller pbf-files (Genererar pbf-filer för topografiska linjer.)
    -img eller image-files (Genererar image filer för topografisk karta.)
    -me eller merge (Slår ihop standardkartan med topografiska linjer.)
    -m eller move (Flyttar standardkarta till /home/osmtest/public_html/garmin/.)
    -m2 eller move2 (Flyttar karta med topografiska linjer till /home/osmtest/public_html/garmin/.)
    -c eller clean (Rensar bort alla filer för Denmark efter att inte gamla filer ska ligga kvar nästa gång du vill skapa en ny karta.)



### Not complete ###
The script is not completely done yet, so there are some missing functions in it right now.

The topographic part needs another script that is right now a separately script, but it will soon be implemented.


### Help & Contact ###
If you need to contact me, you cand find me on IRC on freenode, dalnet, quakenet and oftc as Malmis.
You could also send me an email if you don't know how to use IRC.

Email: mitod1@gmail.com
