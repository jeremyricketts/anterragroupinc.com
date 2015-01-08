anterragroupinc.com
===================

Anterra Group Inc Website code. 

## Master Branch (this one):

This is the source code for building the SiteLeaf template. Install the siteleaf gem, make sure you're on a recent version of non-system ruby, and then updating the website's theme code will look like this:

1. Run `siteleaf auth` and log into the Anterra siteleaf account.
2. git clone this repo.
3. Run `siteleaf theme pull` to make sure you have all the most recent theme changes someone may have made on the SiteLeaf account (there shouldn't be any, unless someone got ballsy and edited them).
3. Once this if there were any differences, commit them to the git repo, just to keep this branch up to date with the theme code. 
4. Make your changes locally and run `siteleaf server` to kick off a local server.
5. Once you're finished, commit the changes again to the master branch and `git push origin master` it up to github. This doesn't actually deploy the theme. 
6. To deploy the theme, run `siteleaf theme push`.
7. Once the theme is deployed, log into SiteLeaf's site an hit the "Publish" button for good measure. SiteLeaf will generate the site and depoy it to this repo, in the `gh-pages` branch.

## gh-pages Branch

This is the branch SiteLeaf will dump the generated site into.
