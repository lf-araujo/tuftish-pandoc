\frontmatter

# Preface

This is destined to be a long front matter text. The text below does not necessarily make any sense, it is just a place holder. It, however, uses all amenities from tuftish-pandoc. This is an attempt to reproduce *some* tufte features plus adding support for R code and graphic capabilities (I have scientific reports and books in mind), but allowing the writer to set linestretch and fonts for whatever s/he wants.

Fullwidth figures are **not** supported, however fullwidth verbatim code **is**. In order to get that effect one can enclose the code snippet between `/fullwbegin /fullwend`. 

The two strongest points of this style is that it can be imported with `mighty_make` with:

```
make fetch THEME="https://github.com/lf-araujo/tuftish-pandoc"
```

This theme supports R code via [pp](https://github.com/CDSoft/pp). You can either add graphics from R code or R output directly into your documents much like `knitr`, but much better as all internationalisation from \LaTeX is supported, together with the cross-reference support from pandoc-crossref.

The inspiration for doing this came from several places. First, from `knitr`, which is excellent for document production but is not the best tool to write in languages other than English. Second, for [Duzin](https://github.com/duzyn/tufte-markdown) who created a tufte "wrapper" in `pp` for pandoc, and finally CDSoft, pp's maintainer, who was nice enough to include R in his preprocessing tool. So be aware that this tool needs [pp](https://github.com/CDSoft/pp) installed.

This is an unfinished project, I am putting out in github so perhaps it can attract some forks. Note that I still have to finish the cover for the book version of this style, but overall it is a good style for scientific reports.