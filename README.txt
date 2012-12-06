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

For adding to a page it needs (in addition to the server-side extension installed):

mw.loader.using('jquery.ui.autocomplete', function() {
	importScriptURI('http://URL.TO/jquery.mw.linksuggest.js'); /* replace with the correct location of jquery.mw.linksuggest.js */
});

It requires ResourceLoader

== NOTE ==

Function _legacyKeydown NEEDS to match the content of jquery.ui.autocomplete.js "keydown.autocomplete" event, in addition to the "var self = this;" at the first line

== TODO ==

* Rewrite it to not depend on jquery.ui.autocomplete.js, since most of its functionality is being overrriden anyway

