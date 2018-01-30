---
layout: page
---

<!-- This document contains the layout/hierarchy for the website.
     Mostly here for personal tracking purposes so I know what's what. -->

This layout was based on the grayscale template:  
http://startbootstrap.com/template-overviews/grayscale
https://github.com/jeromelachaud/grayscale-theme  

_assets: web-related stuff that I want to keep locally but don't want to push up to GitHub  
_drafts: unpublished posts
_includes:
    css       main css files
        - bootstrap.min.CSS   main bootstrap styles
        - graymain.css        grayscale-based css for the main page
        - graypost.css        grayscale-based css for blog area
        - grayscale.css       original grayscale

    <html files>

    head              references CSS files and fonts

    header            navbar  
        // sections of the main page listed in order below
    about             
    projects
    media  
    speaking  
    contact  
    footer   
      // other sections
    base
    contact
    download


_layouts:
  default.html  main layout for the parallax front page of the website
                this is the layout that references all the includes
  page.html     
  post.html   this is a reference layout copied from elsewhere, maybe TPW's site. not to be used for the main layout.
  postlist.html layout for the main list of posts.

  ---

  Headers Structure:
    head.html - main shared header code
    For page
      -style.css - refers to layout >
      -_layouts/stylepost.css
      _includes/headpost.html > refers to css/grayscale.css, boostrap, graymain.css
    For posts
      -stylepost.css - refers to layout >
      -_layouts/style.css
      -_includes/headpage.html > refers to css/grayscale.css, bootstrap, graypost.css

  Surely this can be optimized?
