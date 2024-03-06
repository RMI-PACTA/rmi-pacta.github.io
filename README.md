# rmi-pacta.github.io

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)

<!-- badges: end -->

This is the repository for the RMI-PACTA technical blog. The technical blog is a place to share technical information about the RMI-PACTA project, including the development of relevant R packages, the development of the overall technical ecosystem, and any other technical aspects of the project.

The blog is built using:
- [blogdown](https://github.com/rstudio/blogdown)
- [Hugo](https://github.com/gohugoio/hugo)
- with the [hugo bootstrap theme](https://github.com/filipecarneiro/hugo-bootstrap-theme)

## Writing a new post
To write a blog post, simply create a new markdown file in the `content/post` directory. The file should have a `.md` extension. You can also create R markdown files with a `.Rmd` extension, which must then be knit before building the site.

## Building the site
To build the site, you will need to have Hugo installed. You can install Hugo from the [Hugo website](https://gohugo.io/getting-started/installing/).

### Using Hugo
Once Hugo is installed, you can build the site by running the following command in the terminal:
```
hugo
```

### Using blogdown
You can also build the site using the `blogdown` package. From the R console, run the following command:

```
blogdown::build_site()
```

`blogdown` also allows you to conveniently build `Rmd` files using the `blogdown::build_site(build_rmd = TRUE)` function.

## Serving the site
To view the site, you can run the following command in the terminal:
``` 
hugo server
```
or, from the R console:
```
blogdown::serve_site()
```

## Deploying the site
The site is deployed using GitHub pages. To deploy the site, simply push the changes to the `main` branch of the repository. GitHub actions will take care of the rest.
