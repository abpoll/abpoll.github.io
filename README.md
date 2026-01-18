# Personal webpage for Adam Pollack

<!-- badges: start -->
![Site Status](https://img.shields.io/website?url=http%3A//abpoll.github.io)
<!-- badges: end -->

## Overview

Source code for my [personal webpage](abpoll.github.io), built using [Quarto](https://quarto.org/). An older version of this repository was based on the popular academicpages template, but I find Quarto easier to use and customize. 

## How I set this up

### My 'stack'
- Quarto (system-wide)
- VS Code (and add the Quarto extension)
- Mambaforge (I use `mamba` for speed)
- A project environment (I used `mamba` to create from `environment.yml` in this repo).

### What I did
- I set up Quarto to publish to GitHub pages following the [Publish Action instructions](https://quarto.org/docs/publishing/github-pages.html#publish-command). The set up instructions were a bit tricky but once it's live, I haven't had a problem 
- Created a submodule of a repository called 'bibliography' where I keep one bib file of my publications and another of my conference presentations
- Created the `mamba` environment from `environment.yml`, set up a kernel, and then set up the environment as my Python interpreter in VS Code

## How I make updates

### Local work
- I like to have subdirectories that correspond to each page in my navbar and organize the `.qmd` files in there, typically just an `index.qmd`
- I like using the preview function in VS Code but I also like to checkout the pages I'm working on in different browsers by copy/pasting the localhost url

### Updating webpage
- Always double check my `quarto-web` environment is active
- Always double check my bibliography is updated with `git submodule update --init --recursive`
- I run `quarto render` when I'm happy with my updates (I want my pages that use code to run locally)
- I add, commit, and push changes to my `main` branch
- The `publish.yml` workflow takes care of the rest

## Acknowledgements
I am really grateful for the Quarto developers and the many people who open-source their Quarto projects to provide helpful examples. 

I specifically owe a lot to a few webpages I've drawn heavily from: 

- Vivek Srikrishnan's [personal](https://viveks.me/) and [research group](https://viveks.bee.cornell.edu/) webpages
- James Doss Gollin's research group [webpage](https://dossgollin-lab.github.io/)
- Andrew Heiss's [webpage](https://www.andrewheiss.com/)

## Contact
If for some reason you decide to fork my repository instead of one of theirs, and you run into any trouble, I've probably also run into and figured out how to deal with that issue by now. Please feel free to contact me at [adam-pollack@uiowa.edu](mailto:adam-pollack@uiowa.edu).