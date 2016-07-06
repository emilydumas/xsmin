xsmin: A Minimalist Beamer Theme
================================

This is a beamer template derived from "Execushares" by Kenton
Hamaluik (http://hamaluik.com/posts/better-beamer-themes/).  Many
features of that theme have been removed.  A few minor cosmetic
changes have been made as well.

Status
------

This template is a work in progress and the current version has many
known issues.  Use at your own risk.


Requirements
------------

* xelatex
* Beamer
* tikz
* Adobe's "Source Pro" Fonts (free):
    * [Source Serif Pro](http://store1.adobe.com/cfusion/store/html/index.cfm?store=OLS-US&event=displayFontPackage&code=1966)
    * [Source Sans Pro](http://store1.adobe.com/cfusion/store/html/index.cfm?event=displayFontPackage&code=1959)
    * [Source Code Pro](http://store1.adobe.com/cfusion/store/html/index.cfm?store=OLS-US&event=displayFontPackage&code=1960)

Quick start
-----------

In the linux terminal, a typical command to compile the sample
presentation would be

`xelatex sample.tex`

producing as output `sample.pdf`.

To use xsmin with your own presentation, use documentclass `beamer`
and add the command

`\usetheme{xsmin}`

to your document preamble.  Also copy `beamerthemexsmin.sty` to the
directory containing your tex file, or place this style file in the
xelatex search path.

Known issues
------------

* The title slide is drawn over top of whatever is on slide 1, even if
  that slide is not designated as the title slide.
  
* The square bullets for enumerated or itemized lists do not have the
  correct vertical alignment if a larger font size is used.
  
* The contact info slide in the sample presentation is sometimes not
  rendered correctly.  Recompiling the presentation seems to fix this,
  but the cause is unknown.
  
 * The title slide, frame title, and contact info slide are not beamer
   templates (as they should be), but instead are drawn manually after
   instructing beamer to create a suitable blank area on the slide.


Contributors
------------

David Dumas <david@dumas.io>

The Execushares theme (from which this one was derived) was created by
Kenton Hamaluik.
