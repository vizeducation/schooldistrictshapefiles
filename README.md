# schooldistrictshapefiles

some cleanup and appending on the Census shapefiles for easier consumption by ed research wonks

states with different district types (elementary, secondary, unified) have been appended to the 00_ALL STATES.zip file; just need to crosswalk the FIPS codes.

to retain district type info, you can use a flavor of this IF statement:
IF LEFT([Affgeoid],2)= "95" THEN "Elementary"
ELSEIF LEFT([Affgeoid],2)= "96" THEN "Secondary"
ELSE "Unified"
END
