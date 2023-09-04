# bibliography

This repository contains `.bib` files containing my papers. 
* `my-papers.bib`: papers by me;
* `conferencs.bib`: conference talks and posters by me;

### Add to Project

To add to a project, use:
```
git submodule add -b main https://github.com/vsrikrish/bibliography.git
git submodule init
```  
To pull the latest updates:
```
git submodule update
cd bibliography
git pull
cd ..
```
And to remove:
```
# remove the submodule entry from .git/config
git submodule deinit -f bibliography

# remove the submodule directory from the superproject's modules directory
rm -rf .git/modules/bibliography

# remove the entry in .gitmodules and remove the submodule directory
git rm -f bibliography
```
