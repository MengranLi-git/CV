# CV
My CV for phd application

It is powered by R package [pagedown](https://github.com/rstudio/pagedown) and modified on the basic of [pagedown_cv](https://github.com/ulyngs/pagedown-cv). The original templete is designed by [@ulyngs](https://github.com/ulyngs).

I simplified the workflow of generating a CV through the [pagedown_cv](https://github.com/ulyngs/pagedown-cv) project, changed some CSS style, which made it more suitable for Ph.D. application, and made the pdf document available.

## How to use

Just download the project, open the `CV.rmd` and knit it.

### Indivisual data

A csv document is stored in the `data` filter. Edit the csv as you like. Notice the `date` should take the form of **yyyy-mm-dd**.

### Knit to pdf

`knit: pagedown::chrome_print` should be contained in the head of the `CV.rmd` document. If you don't want a pdf document, then it could be deleted.

If failing to knit to a pdf in the case that R can not find the Chrome browser,just run the `setchrome.R`.

### Sections

The workflow is reading the data csv, transforming the table into suitable form, printing the table via `kable()` function and generating it into html or pdf. 

There are several useful inside codes:

`<br>` change a line

`<span>xxxx</span>` a new style

`<i class="xxxx"></i>` a new icon

The new icon can be found on [Font Awesome](https://fontawesome.com/v5.15/how-to-use/on-the-web/referencing-icons/basic-use)

### CSS

`CSS/CV.css`
