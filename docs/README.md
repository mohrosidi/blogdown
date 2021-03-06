To compile this book, open `index.Rmd` in the RStudio IDE, install the **blogdown** package from Github, and click the RStudio Addin "Preview Book". You should be able to preview the HTML version of the book.

It is trickier to compile it to PDF. You need to install LaTeX. I recommend [TinyTeX](https://yihui.org/tinytex/):

```r
devtools::install_github(c('yihui/tinytex', 'rstudio/rmarkdown'))
tinytex::install_tinytex()
```

Then download and install three fonts from [Google Fonts](https://fonts.google.com/?query=source&selection.family=Alegreya|Alegreya+SC|Source+Code+Pro): Alegreya, Alegreya SC, and Source Code Pro. Run `make pdf` (if `make` is available) or `Rscript _render.R "bookdown::pdf_book"` in the `docs/` directory. Install LaTeX packages if missing. If you're using a Mac with OS X 10.8 or later, install [XQuartz](https://www.xquartz.org).
