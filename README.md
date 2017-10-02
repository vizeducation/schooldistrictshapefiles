# schooldistrictshapefiles

some cleanup and appending on the Census cartographic boundary shapefiles for easier consumption by ed research wonks
(source: https://www.census.gov/geo/maps-data/data/tiger-cart-boundary.html)

states with different district types (elementary, secondary, unified) have been appended to the 00_ALL STATES.zip file; just need to crosswalk the FIPS codes.

to retain district type info, you can use a flavor of this IF statement:
IF LEFT([Affgeoid],2)= "95" THEN "Elementary"
ELSEIF LEFT([Affgeoid],2)= "96" THEN "Secondary"
ELSE "Unified"
END

FIPS Coces:
State; Abbreviation;	FIPS Code	State Name
AL	01	ALABAMA
AK	02	ALASKA
AZ	04	ARIZONA
AR	05	ARKANSAS
CA	06	CALIFORNIA
CO	08	COLORADO
CT	09	CONNECTICUT
DE	10	DELAWARE
DC	11	DISTRICT OF COLUMBIA
FL	12	FLORIDA
GA	13	GEORGIA
HI	15	HAWAII
ID	16	IDAHO
IL	17	ILLINOIS
IN	18	INDIANA
IA	19	IOWA
KS	20	KANSAS
KY	21	KENTUCKY
LA	22	LOUISIANA
ME	23	MAINE
MD	24	MARYLAND
MA	25	MASSACHUSETTS
MI	26	MICHIGAN
MN	27	MINNESOTA
MS	28	MISSISSIPPI
MO	29	MISSOURI
MT	30	MONTANA
NE	31	NEBRASKA
NV	32	NEVADA
NH	33	NEW HAMPSHIRE
NJ	34	NEW JERSEY
NM	35	NEW MEXICO
NY	36	NEW YORK
NC	37	NORTH CAROLINA
ND	38	NORTH DAKOTA
OH	39	OHIO
OK	40	OKLAHOMA
OR	41	OREGON
PA	42	PENNSYLVANIA
RI	44	RHODE ISLAND
SC	45	SOUTH CAROLINA
SD	46	SOUTH DAKOTA
TN	47	TENNESSEE
TX	48	TEXAS
UT	49	UTAH
VT	50	VERMONT
VA	51	VIRGINIA
WA	53	WASHINGTON
WV	54	WEST VIRGINIA
WI	55	WISCONSIN
WY	56	WYOMING
