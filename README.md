Disclaimers
===========

- It seems unfortunately [the HTML5 Document Outline is a dangerous fiction](http://blog.paciellogroup.com/2013/10/html5-document-outline/)
- Be careful about performance through when using such complex selectors in your CSS.

HTML5 Outlines pros & cons
==========================

From [HTML5Doctor's article about Outlines](http://html5doctor.com/outlines/) :

> The document outline is the structure of a document, generated by the document’s headings, form titles, table titles, and any other appropriate landmarks to [map out the document](http://www.w3.org/TR/2002/REC-UAAG10-20021217/guidelines#tech-provide-outline-view). [...] The outlining algorithm has been clearly defined in the [HTML5 spec](http://dev.w3.org/html5/spec/Overview.html#outlines).

It allows web developers to use only `<h1>`s in their content thanks to a hierarchy of sectioning element containing them. This is really useful with Content Management Systems that may generate the same HTML source for several usages.

Unfortunately, most browsers still don't have default CSS rendering for such multi level `<h1>`s.

HTML5 Titles Inception to the rescue
====================================

[HTML5 Titles Inception](https://github.com/nhoizey/HTML5-Titles-Inception) tries to help, with a (not so) little CSS that you can extend.

It shows how to style `<h1>`-`<h3>` elements according to the number of sectioning elements they are embeded into.

Fortunately, tools such as [LESS](http://lesscss.org/) and [SASS](http://sass-lang.com/) exist, so that you don't have to put the whole CSS mess into your files.

Inspiration
===========

HTML5 Titles Inception is inspired by Paul Rouget's [-moz-any selector tutorial](https://hacks.mozilla.org/2010/05/moz-any-selector-grouping/) and  Rob Reyes's [5 levels of Inception](http://www.giantfreakinrobot.com/scifi/5-levels-inception-infographic.html).
