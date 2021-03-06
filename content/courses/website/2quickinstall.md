---
title: Quick Install with Netlify and Github
linktitle: Quick Install with Netlify and Github
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false
menu:
  website:
    parent: 1) Getting Started
    weight: 2

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 2
---

## Ready, Set, Go

There are a few different ways to install and use hugo-academic. I am just going to share with you the path I felt was easiest and most straightforward.

[Click here to install with Netlify](https://app.netlify.com/start/deploy?repository=https://github.com/sourcethemes/academic-kickstart)

1. If you do not have a GitHub or GitLab account you can create one for this purpose. 
2. This process will create a repository called academic-kickstart.
3. Netlify will provide you with a URL which you can customize or you can purchase your own domain name.
4. Netlify will push changes from your GitHub to your webpage automatically. 
5. You can edit your website through GitHub; however we will use GitHub desktop and R Studio to do so. 

## GitHub Desktop

Once you have your GitHub account you will need to download GitHub desktop in order to edit your repository on your desktop using R Studio. 

[Click here to install with GitHub Desktop](https://desktop.github.com/)

1. Locate the GitHub folder for academic-kickstart in your documents and start a R Studio Session with this folder set as your working directory. 
2. Remember that saving changes to your website in this format is a two step process: 
  * Save R document, 
  * Push changes to repository through GitHub Desktop.
3. Now that we have the R Studio project open we can start to edit your website.

## Using Blogdown

1. Install Blogdown in R Studio using `install.packages("blogdown")`
2. Load the package using `library(blogdown)`
3. Build your site using `blogdown::build_site()`
4. Serve the site locally using `blogdown::serve_site()`
5. This will allow your site to show in the viewer portion and display changes you are making to the site. To better view these changes make sure to expand this viewer to an internet explorer window. 

```{r eval=FALSE}
install.packages("blogdown")
library(blogdown)
blogdown::build_site()
blogdown::serve_site()
```
