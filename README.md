
# Steve’s R Markdown Templates

[![](https://www.r-pkg.org/badges/version/stevetemplates?color=green)](https://cran.r-project.org/package=stevetemplates)
[![](http://cranlogs.r-pkg.org/badges/grand-total/stevetemplates?color=green)](https://cran.r-project.org/package=stevetemplates)
[![](http://cranlogs.r-pkg.org/badges/last-month/stevetemplates?color=green)](https://cran.r-project.org/package=stevetemplates)
[![](http://cranlogs.r-pkg.org/badges/last-week/stevetemplates?color=green)](https://cran.r-project.org/package=stevetemplates)

<img src="http://svmiller.com/images/stevetemplates-hexlogo.png" alt="My stevetemplates hexlogo" align="right" width="200" style="padding: 0 15px; float: right;"/>

`stevetemplates` is an R package to help you create lovely R Markdown
documents, primarily for conversion to LaTeX PDFs. They come from [my
suite of R Markdown
templates](https://github.com/svmiller/svm-r-markdown-templates), which
I’m making available as an R package. The impetus behind the R package
is three-fold. First, I’ve always wanted to get something on CRAN just
to say I did it. Two, I’m hopelessly vain and like making my first name
as a prefix for various R-related things (see also:
[`stevemisc`](https://github.com/svmiller/stevemisc) and the forthcoming
`stevedata` as part of the hypothetical and ideally also forthcoming
`steveverse` for all things R and me (i.e. Steve)). Three, it would be
nice to cut down on how clunky my YAML can get and it’d be nice for me
and other users to have one single place to store these templates that
don’t depend on my cornball relative paths.

## Installation

You can install this on CRAN.

``` r
install.packages("stevetemplates")
```

The development version may also have some extra goodies not yet
published on CRAN. You can install the development version of
`stevetemplates` from Github via the `devtools` package. I suppose using
the `remotes` package would work as well.

``` r
devtools::install_github("svmiller/stevetemplates")
```

## Usage

The easiest way to use my templates is within Rstudio. Go to *File &gt;
New File &gt; R Markdown*. Here, select any template you’d like to use.
The version on CRAN should lag behind the development version, but the
development version includes the following templates:

-   [**Steve’s First Article/Manuscript
    Template**](http://svmiller.com/blog/2016/02/svm-r-markdown-manuscript/):
    This is my first article/manuscript template and I made it
    around 2016. I include this as a legacy. I used to use these quite
    often for my manuscripts, though I switched to another template
    (also included in this package). I don’t intend to offer much
    support for this template anymore, but it has lots of goodies
    (e.g. appendix support, suppressing title pages, etc.). You can call
    it in the YAML with `stevetemplates::article`.
-   [**Steve’s 2nd Article/Manuscript
    Template**](http://svmiller.com/blog/2020/09/another-rmarkdown-article-template/):
    This is my second article/manuscript template that I made in
    September 2020. It’s patterned off [the Association for Computing
    Machinery (ACM) LaTeX
    templates](https://www.latextemplates.com/template/acm-publications).
    You can call it in the YAML with `stevetemplates::article2`.
-   [**Steve’s Academic CV
    Template**](http://svmiller.com/blog/2016/03/svm-r-markdown-cv/):
    This is my academic CV template I made in 2016, and I think it’s my
    most popular. It’s certainly the one I see most often in the wild.
    It’s also what I currently use for [my CV](http://svmiller.com/cv/).
    You can call it in the YAML with `stevetemplates::cv`.
-   [**Steve’s Non-Academic Résumé
    Template**](http://svmiller.com/blog/2020/09/rmarkdown-template-non-academic-resume/):
    This is an addition I made in 2020 to my suite of R Markdown
    templates. It’s a bit clunky, but it’s useful and markup-light for
    non-academic résumés. You can call it in the YAML with
    `stevetemplates::resume`.
-   [**Steve’s Memo
    Template**](http://svmiller.com/blog/2019/06/r-markdown-memo-template/):
    I created this for a memo I needed to write in 2019. You can call it
    in the YAML with `stevetemplates::memo`.
-   **Steve’s Statement Template**: I created this template in 2016 (I
    believe). I use it for writing various “statements” (e.g. [my
    research
    statement](http://svmiller.com/docs/svm-research-statement.pdf),
    statement of [teaching
    philosophy](http://svmiller.com/docs/svm-teaching-philosophy.pdf))
    when applying for jobs. I also use it for miscellaneous university
    busy work. You can call it in the YAML with
    `stevetemplates::statement`.

The user should notice that the YAML contains the functions (loaded in
this package) to compile these documents. They are basic wrappers for
`rmarkdown::pdf_document`. Please consult the corresponding posts and
[the template
repository](https://github.com/svmiller/stevetemplates/tree/master/inst/rmarkdown/templates)
for rudimentary examples and the underlying code to help guide your
usage.
