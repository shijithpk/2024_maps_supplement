# 2024_maps_supplement
Supplementing Datameet maps with some newer, updated ones for the 2024 elections

The maps in the [Datameet repo](https://github.com/datameet/maps) meet most of my needs, but some areas like Assam and J&K still have pre-delimitation parliamentary seat borders.

This is an attempt to provide maps that can substitute some of the outdated ones in the Datameet repo.

These geojsons aren't research quality, but I think they're good enough for the purpose of visualising on websites.

### Done
* [Sikkim assembly seat map](sikkim_assembly_updated.geojson)
* [Assam Lok Sabha seat map](assam_ls_new_borders.geojson)
* [J&K Lok Sabha seat map](j_and_k_ls_new_borders.geojson)
* [Ladakh Lok Sabha seat map](ladakh_ls_new_borders.geojson)
* [India Lok Sabha seat map](india_ls_seats_545.geojson) (incorporating the newer borders of all the states above. It has 2 extra features for areas in J&K claimed by India but administered/controlled/occupied by others.)
* [India Lok Sabha seat map](india_ls_seats_543.geojson) (same as above, but with 543 features, one for each Lok Sabha seat)

### Pending
* J&K assembly seat map (will do this in July)

### Notes
* Source maps used for sikkim, assam, ladakh, j and k are in the **source maps** folder
* The main source maps were taken from this [press note pdf](https://elections24.eci.gov.in/docs/press-note-no-23.pdf) from the election commission
  * The various maps in the pdf can be extracted as svgs if you want updated maps for other states/UTs.
* Other source maps were taken from the websites of the state election commissions
* Areas in J&K claimed by India but administered/controlled/occupied by others have been assigned the *ls_seat_code* value of '999'
  * Have created two India maps to allow people the freedom to decide how to deal with those occupied areas.
  * If you don't want to mess with all that and just want an India map with 543 features, one feature for each seat, use [india_ls_seats_543.geojson](india_ls_seats_543.geojson)
* Because the maps were created by georeferencing images in QGIS, some of the borders will be off, so use at your own risk.
  * The quality of the all-India Lok Sabha seat maps could be better, will see if I can improve them, no promises though.
  * Hopefully someone from the GIS community in India will step up and create a more accurate seat map that we can use instead. Will link to it *here* if anyone does.
* If someone comes across this online, and wants to create a better map, see if you can build one from the taluk up for J&K and Assam.
  * Because even if you georeference the election commission images and create slightly better maps than the ones in this repo, it will still just represent *marginal gains* in accuracy.
  * Building lok sabha seats from the taluk up is time-consuming, but that should be the next step.
* If you want to use these geojsons for visualisation on the web, its best to convert them to topojsons, they will be smaller in file size.




