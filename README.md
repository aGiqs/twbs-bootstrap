# twbs-bootstrap versions

Versions of getbootstrap.com


this is a repo to hold different versions of bootstrap you may need.

This master branch only hold this readme to upgrade the branches


# ready to run files
Downloaded from http://getbootstrap.com/ and set to the "packages" branch to 
have several versions an application may need.
If you want several versions this will be your primary branch to choose
    # git checkout packages

If you just need a special version then checkout the branch you need or create
a new branch including the version you want.
If you need several versions? Then merge it to the packages branch an switch
back to the packages branch.



# Examples/ Howto add new versions

## branch master
    ./README.txt (copy of this readme)


## branch of vA-B-C
    ./vA.B.C/ - QueryBuilder src and dist files
    ...
    ./vA.B.C/README.txt (README of QueryBuilder vA.B.C)
    ./README.txt (copy of this readme)


If a new version exists and you need it globaly/ in packages branch:
Don't drop other versions! Add your version to the packages branch or create
and checkout your version.

Eg: You need verion 2.0.1 system wide:
checkout the master branch and create a new branch: "v2-0-1" (branches needs - NOT dots!)
create a folder: mkdir v2.0.1/
Download the file *.js/*.css to v2.0.1/
commit & push the new version branch

Then checkout the "packages" branch and merge your version into it. 
Result (Example):
# packages branch

    ./vA.B.C/bootstrap.js
    ./vA.B.C/README.txt
    ./v2.0.1/bootstrap.js
    ./v2.0.1/README.txt
    ./README.txt                        #(copy of this readme on creation time)
    ./plugins/v1/**                     # Mixed plugins for bootstrap v1.*
    ./plugins/v1/pluginname/v1****/     # Mixed versions for pluginname
    
# plugins to package

E.g:
    remotes/origin/HEAD -> origin/master
    remotes/origin/master
    remotes/origin/packages
    remotes/origin/plugin-v1-pluginnameA-v1-2-3
    remotes/origin/plugin-v1-pluginnameB-v3-4-5
    remotes/origin/plugin-v1-pluginnameC-v6-7-8
    remotes/origin/v1-1-1
    remotes/origin/v1-2-2
    remotes/origin/v3-1-1



# Changelog

    2021
        - Adds version 3.3.1
        - init repo

