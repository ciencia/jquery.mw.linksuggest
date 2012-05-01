jQuery MediaWiki LinkSuggest

The client-side of Extension:LinkSuggest[1], an extension of MediaWiki[2].

It suggests / autocompletes internal links and templates when typing the start of a link "[[" or a template "{{" based on existing page titles.

It requires jQuery and jquery.ui.autocomplete.js, which in turn requires:
 *	jquery.ui.core.js
 *	jquery.ui.widget.js
 *	jquery.ui.position.js

External links:

 [1] http://www.mediawiki.org/wiki/Extension:LinkSuggest
 [2] http://www.mediawiki.org/

== TODO ==

* Ensure that it works with ResourceLoader
* Rewrite it to not depend on jquery.ui.autocomplete.js, since most of its functionality is being overrriden anyway

