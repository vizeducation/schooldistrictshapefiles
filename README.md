# schooldistrictshapefiles

some cleanup and appending on the Census cartographic boundary shapefiles for easier consumption by ed research wonks
(source: https://www.census.gov/geo/maps-data/data/tiger-cart-boundary.html)

states with different district types (elementary, secondary, unified) have been appended to the 00_ALL STATES.zip file; just need to crosswalk the FIPS codes.

to retain district type info, you can use a flavor of this IF statement:
IF LEFT([Affgeoid],2)= "95" THEN "Elementary"
ELSEIF LEFT([Affgeoid],2)= "96" THEN "Secondary"
ELSE "Unified"
END

FIPS Codes:
<ul>
	<li>State Abbreviation	FIPS Code	State Name</li>
	<li>AL	01	ALABAMA</li>
	<li>AK	02	ALASKA</li>
	<li>AZ	04	ARIZONA</li>
	<li>AR	05	ARKANSAS</li>
	<li>CA	06	CALIFORNIA</li>
	<li>CO	08	COLORADO</li>
	<li>CT	09	CONNECTICUT</li>
	<li>DE	10	DELAWARE</li>
	<li>DC	11	DISTRICT OF COLUMBIA</li>
	<li>FL	12	FLORIDA</li>
	<li>GA	13	GEORGIA</li>
	<li>HI	15	HAWAII</li>
	<li>ID	16	IDAHO</li>
	<li>IL	17	ILLINOIS</li>
	<li>IN	18	INDIANA</li>
	<li>IA	19	IOWA</li>
	<li>KS	20	KANSAS</li>
	<li>KY	21	KENTUCKY</li>
	<li>LA	22	LOUISIANA</li>
	<li>ME	23	MAINE</li>
	<li>MD	24	MARYLAND</li>
	<li>MA	25	MASSACHUSETTS</li>
	<li>MI	26	MICHIGAN</li>
	<li>MN	27	MINNESOTA</li>
	<li>MS	28	MISSISSIPPI</li>
	<li>MO	29	MISSOURI</li>
	<li>MT	30	MONTANA</li>
	<li>NE	31	NEBRASKA</li>
	<li>NV	32	NEVADA</li>
	<li>NH	33	NEW HAMPSHIRE</li>
	<li>NJ	34	NEW JERSEY</li>
	<li>NM	35	NEW MEXICO</li>
	<li>NY	36	NEW YORK</li>
	<li>NC	37	NORTH CAROLINA</li>
	<li>ND	38	NORTH DAKOTA</li>
	<li>OH	39	OHIO</li>
	<li>OK	40	OKLAHOMA</li>
	<li>OR	41	OREGON</li>
	<li>PA	42	PENNSYLVANIA</li>
	<li>RI	44	RHODE ISLAND</li>
	<li>SC	45	SOUTH CAROLINA</li>
	<li>SD	46	SOUTH DAKOTA</li>
	<li>TN	47	TENNESSEE</li>
	<li>TX	48	TEXAS</li>
	<li>UT	49	UTAH</li>
	<li>VT	50	VERMONT</li>
	<li>VA	51	VIRGINIA</li>
	<li>WA	53	WASHINGTON</li>
	<li>WV	54	WEST VIRGINIA</li>
	<li>WI	55	WISCONSIN</li>
	<li>WY	56	WYOMING</li>
</ul>
