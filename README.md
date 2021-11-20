# Junction/Edge Rename script - SUMO net xml file

The Map (***map.osm file***) is downloaded from Open Street Map and is then converted into a SUMO Network (***saltlake.net.xml***).
>Command used: netconvert --osm-files map.osm -o saltlake.net.xml

Execute the file ***index.py*** to obtain the desired result. The final output sumo network file is ***saltlake_final.net.xml***.

The Junction ids in the ***saltlake.net.xml*** file (NET file) are renamed as “a_id-number” and internal
junction ids as “b_id-number” using the python script ***junction-id-modification.py***. 
After the Junction ids are renamed, the Edge ids are renamed as “fromJunction-id_toJunction-id” 
and internal edge ids as "ie_id-number" using the python script ***edge-id-modification.py***.

Make sure SUMO is installed.
Python version used - v3.7.6
