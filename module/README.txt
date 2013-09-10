/*
cu_customsearch is a module to replace GooSACUL. Instead of using the
Google Search Appliance, it uses Google Custom Search 
http://www.google.com/cse/
It is a plugin replacement for goosacul - the old search forms should work
without modification.

It requires another module google_cse and takes advantage of its admin interface
/admin/settings/google_cse

Installation:
	install google_cse
	enable Search, Google CSE and Google CSE search
	in the google_cse admin at /admin/settings/google_cse
		set Google Custom Search Engine ID to the one from your google custom search
			Cornell Library Sites:  017399541683802799304:1axhejcyau8
		set Search results page title - used for page title by cu_customsearch
		set SiteSearch domain to (your site domain) Search this site
		uncheck Search results "Add to Google" Google Gadget
	install and enable cu_customsearch
	if you have an actual page /search/cul_gsa get rid of it

Use:
	banner search boxes should just work
	note: the Cornell search option now redirects to the Cornell.edu site's search
	/cu_search - general search results interface
	/cu_search?qp=hour&sitesearch=www.library.cornell.edu
		preloads 'hours' into search string
		preselects the 'Search this site' option
	Blocks:
		Google CSE
		Google CSE results
		Cornell Custom Search Form
		
Note:
	sitesearch domains must be part of your 'Custom Search Element' sites list
	you can list more than one SiteSearch domain in /admin/settings/google_cse
		the search interfaces lists them in a popup instead of radios

-JGReidy jgr25 2/22/2012
*/