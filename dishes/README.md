## Dish datasets

It's a bit of a vague distinction, though I feel like it's important to have an understanding of a 'dish' -- as an idea of a named food that exists in relation to other dishes, and participates . A recipe is an instance of an instruction that captures how to *make* a dish (named or unnamed), while a dish is a concept, free to associate with other entites. A 'dishes' dataset deals with other information: what other dishes, cuisines, holidays, meals, events, places or other practices are associated with this dish? What dishes exist in the world? How is a dish described? Necessarily, there's some overlap here, but I feel like it's nice to have both.

This [repository](https://github.com/agnescameron/related-dishes) contains links to:

* A dataset of [relationships between dishes](https://github.com/agnescameron/related-dishes), scraped using a wiki crawler in the 'See Also' section
* A [dataset of dishes](https://github.com/agnescameron/wiki-dish-scraper) (needs to be cleaned!), scraped by scraping the wikipedia lists of dishes
* A [dataset of different dishes from cooking sites](https://github.com/fakela/recipe-links-crawler), scraped using selenium and scrapy

See also:

In [recipes](../recipes), scraped datasets of multiple recipes for a particular dish (e.g. okonomiyaki, meatballs).
The [Grubhub restaurant graph](https://pydata.org/nyc2019/schedule/presentation/54/discover-your-latent-food-graph-with-this-1-weird-trick/) does some interesting work with dish embeddings.

### Status

* Search: what are the sources?
	* it would be great to get a dataset of meals (e.g. dishes to eat together). For example, the website [Archana's Kitchen](https://www.archanaskitchen.com/egg-curry-recipe) always adds a 'serve with' suggestion to the end of their recipes
	* different taxonomies of dishes -- wet/dry, heating/cooling, seasonal, religious
	* [Taste Atlas](tasteatlas.com/) -- an index of different national dishes
	* extract more data from descriptions on wikipedia
	* smaller datasets around particular places, holidays etc: e.g. 
* Schematise: what is the schema for this dataset?
	* related dishes schema
	* dishes schema
* ↱ Parse ↴: what data has been scraped?
	* A dataset of related dishes, scraped from wikipedia
		* related-dishes might be incomplete, but will not need much cleaning
		* could be made more complete by crawling the cleaned dishes dataset
	* A dataset of all wikipedia pages included in lists of 'dishes'
		* larger, needs cleaning before usable
		* includes descriptions: could do some ML on these to auto-find the non-dishes
* Reconcile: how does this data map onto existing datasets?
	* Want to scrape 5 recipes for each dish in the dish dataset, matching into the recipe schema
* Collect: is it all in one place?
* Query: what questions could this collection answer?
	* what's a similar dish to *X*
	* what should I make for Easter lunch?
	* 
* Transform and Export: what format is it in?
	* the related recipes are in Neo4j and json format
	* the lists of dishes are in JSON format
* Test and Validate: have we done any cleaning/validating/testing?
	* not yet...

