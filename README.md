# Contributing

For small edits you can edit via the GitHub interface, simply navigate to the
file and choose the edit option. Most content is in markdown format and GitHub
provides a preview option.

For more involved edits build the Jekyll site locally:

* Install the dependancies by following along with [setting up your pages site
  locally with Jekyll][1]
* Clone the repositiory and checkout the `gh-pages` branch.
* Make your changes and test with:

```bundle exec jekyll serve``` 

## Updating training courses

To update the training course table you need to edit
`_data/osgeouk_training.csv`. Once you've edited the CSV please make sure it's
valid using https://csvlint.io/.

## Pushing to the live site

Once you're happy with your changes and wish to publish them:

If you don't have commit access to the repository create a pull request via GitHub.

If you have commit access:

* Pull any upstream changes, merge and test again
* Commit your changes and push to the gh-pages branch
* Wait a few minutes for the Jekyll site to be built by GitHub Pages :-)

[1]: https://help.github.com/articles/setting-up-your-pages-site-locally-with-jekyll/
