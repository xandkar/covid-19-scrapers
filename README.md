COVID-19 scrapers
=================

Quick and dirty. Likely to break as soon as data source HTML structure changes.

Example usage
-------------
	$ ./fetch-case-count-usa-ny -h
	Usage: ./fetch-case-count-usa-ny [OPTION | LOCATION]

	OPTION = -h | --all
	LOCATION =
		Albany
		Allegany
		Broome
		Clinton
		Delaware
		Dutchess
		Erie
		Greene
		Herkimer
		Monroe
		Montgomery
		Nassau
		New York City
		Onondaga
		Ontario
		Orange
		Putnam
		Rensselaer
		Rockland
		Saratoga
		Schenectady
		Suffolk
		Sullivan
		Tioga
		Tompkins
		Ulster
		Westchester
		Wyoming

	Default LOCATION:
		New York City

	$ ./fetch-case-count-usa-ny 2> /dev/null
	644

	$ ./fetch-case-count-usa-ny 'New York City' 2> /dev/null
	644

	$ ./fetch-case-count-usa-ny --all 2> /dev/null
	1    Broome
	1    Clinton
	1    Delaware
	1    Herkimer
	1    Montgomery
	1    Ontario
	1    Rensselaer
	1    Sullivan
	1    Tioga
	1    Wyoming
	2    Allegany
	2    Greene
	2    Onondaga
	2    Putnam
	2    Tompkins
	5    Schenectady
	7    Erie
	8    Ulster
	9    Saratoga
	10   Monroe
	15   Orange
	16   Dutchess
	22   Rockland
	23   Albany
	84   Suffolk
	131  Nassau
	380  Westchester
	644  New York City

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
