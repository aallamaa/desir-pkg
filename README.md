# Debian desir packaging

desir [1] is an alternative redis library w/o some of the funny thread related code.

# How to build

1. Add upstream: git remotes:

      git remote add upstream ../desir
      git remote update

2. Build (unsigned in this case)

      git-buildpackage --git-export-dir=../build/ --git-builder="debuild -uc -us -i -I" 


[1]
https://github.com/aallamaa/desir