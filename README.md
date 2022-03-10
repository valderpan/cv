# cv
My CV

## My pagedown rendered CV

This repo contains the source-code and results of my CV built with the [pagedown package](https://pagedown.rbind.io) and a modified version of the 'resume' template. 

The main files are:

- `index.Rmd`: Source template for the cv, contains a variable `PDF_EXPORT` in the header that changes styles for pdf vs html. 
- `index.html`: The final output of the template when the header variable `PDF_EXPORT` is set to `FALSE`.
- `WeiDong_CV.pdf`: The final exported pdf. 
- `positions.csv`: A csv with columns encoding the various fields needed for a position entry in the CV. A column `section` is also available so different sections know which rows to use.


The source code was derived from <https://github.com/nstrayer/cv>, with modifications:

+ add `order` column in `positions.csv` to adjust item order.
+ remove `time` if it is identical to previous item.
+ add citation stats.
