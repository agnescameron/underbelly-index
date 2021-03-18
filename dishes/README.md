## Dish datasets

It's a bit of a vague distinction, though I feel like it's important to have an understanding of a 'dish' -- as an idea of a named food that exists in relation to other dishes, and participates . A recipe is an instance of an instruction that captures how to *make* a dish (named or unnamed), while a dish is a concept, free to associate with other entites. A 'dishes' dataset deals with other information: what other dishes, cuisines, holidays, meals, events, places or other practices are associated with this dish? What dishes exist in the world? How is a dish described? Necessarily, there's some overlap here, but I feel like it's nice to have both.

### Status

* Search: what are the sources? are there external datasets?
	* it would be great to get a dataset of meals (e.g. dishes to eat together). For example, the website [Archana's Kitchen](https://www.archanaskitchen.com/egg-curry-recipe) always adds a 'serve with' suggestion to the end of their recipes
	* different taxonomies of dishes -- wet/dry, heating/cooling, seasonal, religious
	* [Taste Atlas](tasteatlas.com/) -- an index of different national dishes
	* wikipedia information
* Schematise: what is the schema for this dataset?
	* related dishes schema
	* dishes schema
* ↱ Parse ↴: what data has been scraped?
	* A dataset of related dishes, scraped from wikipedia
		* related-dishes might be incomplete, but will not need much cleaning
	* A dataset of all wikipedia pages included in lists of 'dishes'
		* larger, needs cleaning before usable
		* includes descriptions: could do some ML on these to auto-find the non-dishes
* Reconcile: how does this data map onto existing datasets?
	* Want to scrape 5 recipes for each dish in the dish dataset, matching into the recipe schema
* Collect: is it all in one place?
* Query: what questions does this collection answer?
	* what's a similar dish to *X*
* Transform and Export: what format is it in?
	* 
* Test and Validate: have we done any cleaning/validating/testing?
	* 

This [repository](https://github.com/agnescameron/related-dishes) contains links to:

* A dataset of relationships between dishes, scraped using a wiki crawler in the 'See Also' section
* A dataset of dishes (needs to be cleaned!), scraped by scraping the wikipedia lists of dishes
* A dataset of related dishes scraped using Selenium and Scrapy scripts


collections of recipes for specific dishes:
* [ramen](https://docs.google.com/document/d/1qLPoLxek3WLQJDtU6i3300_0nNioqeYXi7vESrtNvjQ/edit)

