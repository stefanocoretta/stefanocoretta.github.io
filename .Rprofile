source("renv/activate.R")

options(blogdown.hugo.server = c('-D', '-F', '--navigateToChanged', '--ignoreCache'))
options(blogdown.author = "Stefano Coretta")
options(blogdown.serve_site.startup = FALSE)

my_build <- function() {
  blogdown::build_site(build_rmd = blogdown::filter_md5sum)
}

options(blogdown.hugo.version = "0.120.4")
