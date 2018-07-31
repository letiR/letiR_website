## inSileco blogdown

[![Build Status](https://travis-ci.org/inSileco/inSileco.github.io.svg?branch=dev)](https://travis-ci.org/inSileco/inSileco.github.io)
[![Build status](https://ci.appveyor.com/api/projects/status/kxa7ht9m3b1eke22?svg=true)](https://ci.appveyor.com/project/KevCaz/insileco-github-io)


The overarching goal of this blog is quite straightforward: tackle challenges
and opportunities provided by this new era of open-access and computationally
intensive research in the field of ecology.



### Getting started

#### Install blogdown

```r
if(!require(devtools)) install.packages('devtools')
devtools::install_github('rstudio/blogdown')
```

If you want more info on how this package works, have a look at the blogdown [documentation](https://bookdown.org/yihui/blogdown/), you can also have
a quick look at [this blog post](https://blog.rstudio.com/2017/09/11/announcing-blogdown/).

#### Deploy the server

0. Make sure you're at the `HEAD` of the `dev` branch and in the inSileco.github.io folder.
1. Open a terminal and first install Hugo (if not installed already): `Rscript -e 'blogdown::install_hugo()'`
2. Then, run: `Rscript -e 'blogdown::serve_site()'`
3. Site is available at `http://127.0.0.1:4321` from your browser.

If any changes are made on source files, the site will be autogenerated and changes will be displayed at the `localhost` address (`http://127.0.0.1:4321`).


#### Write your own post

0. Clone the repo, make sure your at the `HEAD` of the `dev` branch and in the inSileco.github.io folder;
1. create a new branch (choose a new that reflects what you are adding, here I chose `sppost`) `git branch sppost`;
2. switch branch: `git chekout sppost`;
3. create a new empty post with `Rscript -e 'blogdown::new_post('MY_TITLE')'` in
you terminal, or `blogdown::new_post('MY_TITLE')` after opening R (again the
working directory must be the root of this repo); alternatively, use do `hugo new post/yourpost.Rmd`
which will use the [archetype](https://gohugo.io/content-management/archetypes/);
`post.Rmd`;
4. push your new branch to GitHub and open a new PR
5. assign it to a reviewer;
6. the reviewer (that might be yourself) squash and merge the post;
7. do not forget to pull the `dev` branch once all is done.



#### Colors

- Main: "#3fb3b2";
- Yellow-logo: "#ffdd55";
- red code: "#c7254e";
- blue twitter: "#1b95e0";
- purple kevcaz: "#8555b4"
- So the palette is `c("#3fb3b2". "#ffdd55", "#c7254e", "#1b95e0", "#8555b4")`


#### Badges

- ![](https://img.shields.io/badge/inSileco-InDevelopment-3fb3b2.svg) for posts that still require some work.

- ![](https://img.shields.io/badge/inSileco-UnderReview-ffdd55.svg) for posts that have reached at certain level of quality and submitted to the review of members of the blog.


#### JS/CSS libraries added

- [jQuerryUI](https://jqueryui.com/)
- [Disqus](https://disqus.com/)
- [Tocify](http://gregfranko.com/jquery.tocify.js/)
- [Academicons](https://jpswalsh.github.io/academicons/)
- [Font Awesome 4.7](https://fontawesome.com/v4.7.0/)
