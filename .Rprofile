source("renv/activate.R")

options(blogdown.hugo.server = c('-D', '-F', '--navigateToChanged', '--ignoreCache'))
options(blogdown.author = "Stefano Coretta")

my_build <- function() {
  blogdown::build_site(build_rmd = blogdown::filter_md5sum)
}
