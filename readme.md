# jQuery Autocomplete
My fork of Devbridge's jQuery autocomplete widget has some modifications made to it that improve usability.

## New options
* `fnGetSuggestions`: Allows you to override the retrieval of suggestions (usually done from a URL using AJAX) with a callback. This callback passes in all relevant `params` options (including `params.query`) and expects a list of pairs with `{ suggestion, data }` within them. If your function isn't re-entrant (not sure why that would be), make sure to disable caching or you'll get bizarre behavior when the autocomplete refuses to update.