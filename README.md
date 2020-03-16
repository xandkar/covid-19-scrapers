COVID-19 scrapers
=================

Quick and dirty. Likely to break as soon as data source HTML structure changes.

Example usage
-------------
	$ fetch-case-count-usa-ny -h
	Usage: fetch-case-count-usa-ny [LOCATION]

	LOCATION =
		Albany
		Broome
		Delaware
		Dutchess
		Erie
		Greene
		Herkimer
		Monroe
		Montgomery
		Nassau
		Orange
		Putnam
		Rockland
		Saratoga
		Schenectady
		Suffolk
		Tioga
		Tompkins
		Ulster
		Westchester
		New York State (Outside of NYC)
		New York City:
		Total Positive Cases (Statewide)

	Default LOCATION:
		New York City:

	$ fetch-case-count-usa-ma -h
	Usage: fetch-case-count-usa-ma [LOCATION]

	LOCATION =
		Boston:
		Massachusetts:

	Default LOCATION:
		Boston:

	$ fetch-case-count-usa-ny 2> /dev/null
	329

	$ fetch-case-count-usa-ma 2> /dev/null
	29

	$ fetch-case-count-usa-ny 'Total Positive Cases (Statewide)' 2> /dev/null
	729

	$ fetch-case-count-usa-ma 'Massachusetts:' 2> /dev/null
	164
