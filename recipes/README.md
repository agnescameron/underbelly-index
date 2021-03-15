## Recipe datasets

This [repository](https://github.com/agnescameron/food_schemas) contains:

* Different scripts for scraping recipes 
* Schema generated for the scraped data using FOODON ontology
* Graph database (Neo4j) that satisfies the schema created.

### Status:

* Search:
	* crawling search engines for families of *flexible recipes* from different sources
		* meatballs
		* okonomiyaki
		* [borscht](https://github.com/agnescameron/food_schemas/blob/master/sources/borschts.txt)
	* existing datasets:
		* Yummly-25k
		* Cookpad
		* New York Times (sshh)
	* aggregator sites:
		* Yummly
		* Cookpad
		* AllRecipes
* Schematise: what is the schema for this dataset?
	* draft schema here
* ↱ Parse ↴: which sources have been scraped?
	* Yummly
	* Cookpad did not allow Selenium scraper
	* Allrecipes
* Reconcile: how does this data map onto existing datasets?
	* links ingredients to foodKG entities
* Collect: is it all in one place?
	* all scripts and versioned sample datasets are contained in this [repository](https://github.com/agnescameron/food_schemas)
* Query: what questions could this collection answer?
	* what ingredients are included in X recipe?
	* what is a recipe for X?
	* how many recipes for X contain Y ingredient?
	* what ingredients are commonly included in X?
* Transform and Export: what format is it in?
	* in Neo4j (an older script can also produce linked SQLite data)
* Test and Validate: have we done any cleaning/validating/testing?
	* improved cleaning 
