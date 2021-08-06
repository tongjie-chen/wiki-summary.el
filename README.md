## wiki-summary.el

[![MELPA](http://melpa.org/packages/wiki-summary-badge.svg)](http://melpa.org/#/wiki-summary)

Grab the Wikipedia summary for a term and display the result in a
buffer. Inspired by [WikiTerm][wikiterm].

Currently this exports two functions:

 * `wiki-summary` which will interactively prompt you for the string
of the page title and gives back the information in a buffer
`*wiki-summary*`

 * `wiki-summary-insert` which will interactively prompt you for the string
of the page title and insert (or barf if read only) the summary into the current buffer at point.

You can specify a language encoding (as per the URL for that language) with `M-x customize-variable` and `wiki-summary-language-string`.

[wikiterm]: https://gist.github.com/thedouglenz/193defdb711e0e54d68a

Improved from https://github.com/jozefg/wiki-summary.el by adding
1. Summary image if the wiki page has one
2. Highlight the queried word
3. Fallback to Wikipedia webpage when ambiguious
4. Fallback to Google search when the term is not in Wikipedia
