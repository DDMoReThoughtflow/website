# website
Website for Thoughtflow Community Group

## To make changes to the website using RStudio's blogdown:
1.	Install the blogdown package from Github: https://github.com/rstudio/blogdown . If you have devtools installed you can type: devtools::install_github('rstudio/blogdown').
2.	Install Hugo: blogdown::install_hugo()
3.	Clone the website repository from Github.
4.	Make changes / content.
  *	Static pages should go in /content/page/
  *	Blog posts should go in /content/post/
    *	Note that there’s a date / time stamp for blog posts. I guess if the actual time is after that date / time it’ll “go live”.
  *	Content can be .Rmd or .md pages, although watch that the header format is different for both! You can embed R code (or other coding language) in .Rmd files. Markdown .md files should not have executable code. With .Rmd, the code is run and code with output is embedded in the .md file before rendering. So eventually everything goes .md to .html.
  *	Save changes.
  *	Test changes via blogdown::serve_site() or alternatively blogdown::build_site()
  *	You can make changes to config.toml in the top directory to change the baseurl, theme, author list, add Google Analytics, change the top navigation pane etc. BUT DO SO CAREFULLY!
5.	Add new content to git.
6.	Commit with commit message.
7.	Push to Github.
