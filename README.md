# xmipp-bundle
Xmipp bundle repo with submodules to all new repositories

The main goal of this repo is to facilitate the installation of Xmipp, 
that is now splitted into 3 repositories: xmipp, xmippCore and xmippViz.
Each of them are treated here as submodules.

A nice tutorial for submodules can be found here:

https://git-scm.com/book/en/v2/Git-Tools-Submodules

## Tips

### Clone all submodules recursively

git clone --recurse-submodules git@github.com:delarosatrevin/xmipp-bundle.git

### Add a new submodule
git submodule add git@github.com:I2PC/xmipp-repo.git

### Updating all submodules to the lastest in "devel"
git submodule foreach "(git checkout devel; git pull --prune)&"
