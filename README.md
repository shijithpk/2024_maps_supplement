# 2024_maps_supplement
Supplementing Datameet maps with some newer, updated ones for the 2024 elections

The maps in the [Datameet repo](https://github.com/datameet/maps) meet most of my needs, but some areas like Assam and J&K still have pre-delimitation parliamentary seat borders.

This is an attempt to provide maps that can substitute some of the outdated ones in the Datameet repo.

These geojsons may not be research quality, but I think they're good enough for the purpose of visualising on websites.

### Done
* [Sikkim Assembly seat map](sikkim_assembly_updated.geojson)
* [Assam Lok Sabha seat map](assam_ls_new_borders.geojson)
* [J&K Lok Sabha seat map](j_and_k_ls_new_borders.geojson)
* [Ladakh Lok Sabha seat map](ladakh_ls_new_borders.geojson)
* [India Lok Sabha seat map 1](india_ls_seats_545.geojson) (incorporates new seat borders for Assam and J&K. Has 2 extra features for areas in J&K that technically aren't part of any seat but are needed to show India as a whole.)
* [India Lok Sabha seat map 2](india_ls_seats_543.geojson) (same as above, but with 543 features, one for each Lok Sabha seat. Here the 2 extra features have been merged with existing seats.)

### Pending
* J&K assembly seat map (will do this in July)

### Notes
* If you want to use these geojsons for visualisation on the web, its best to convert them to topojsons, they will be smaller in file size.
* Source maps used for sikkim, assam, ladakh, j and k are in the [source_maps](source_maps) folder
* The main source maps were taken from this [press note pdf](https://elections24.eci.gov.in/docs/press-note-no-23.pdf) from the election commission
	* The various maps in the pdf can be extracted as svgs if you want updated maps for other states/UTs.
* Other source maps were taken from the websites of the state election commissions
* Areas in J&K claimed by India but administered/controlled/occupied by others have been assigned the *ls_seat_code* value of '999'
	* Have created two India maps. The first one [India Lok Sabha seat map 1](india_ls_seats_545.geojson) lets you decide how to deal with these other areas.
	* If you don't want to mess with anything and just want an India map with 543 features, one feature for each seat, use [India Lok Sabha seat map 2](india_ls_seats_543.geojson)
* Because the maps were created by georeferencing images in QGIS, the international borders will be off, so use at your own risk.
	* The quality of the all-India Lok Sabha seat maps could be better, will see if I can improve them, no promises though.
	* Hopefully someone from the GIS community in India will step up and create a more accurate seat map that we can use instead. Will link to it *here* if anyone does.
* If someone comes across this repo online, and wants to create a better map, see if you can build one from the taluk up for J&K and Assam.
	* Because even if you georeference the election commission images and create slightly better maps than the ones in this repo, it will still just represent *marginal gains* in accuracy.
	* Building lok sabha seats from the taluk up is time-consuming, but that should be the next step.
	* As a starting point, you can go through govt. gazette notifications (J&K ones [are here](https://ceojk.nic.in/DELIMI_FINAL.htm)). They have lists of which districts/taluks/tehsils of a state are in which lok sabha seat etc.

### Corrections
* Apr 20, 2024 -- Thanks to Srinivasan Ramani of Hindu for pointing this out, had interchanged the names and election commission ids of two lok sabha seats in Assam -- "Diphu (ex Autonomous District)" and "Kaziranga (ex Kaliabor)". They should be associated with the right seats now. 




