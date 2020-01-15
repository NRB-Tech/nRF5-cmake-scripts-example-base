This is the base project template for [nRF5-cmake-scripts-example](https://github.com/NRB-Tech/nRF5-cmake-scripts-example).

To recreate this from an empty directory:

```shell
# create the directory
mkdir "example"
cd example
# init git
git init
# fetch boilerplate .gitignore
curl https://www.gitignore.io/api/linux,macos,cmake,clion,python,windows -o .gitignore
# append project-specific gitignore additions
echo "

toolchains
cmake-build-*
keys
" >> .gitignore
# fetch the required submodule
git submodule add https://github.com/NRB-Tech/nRF5-cmake-scripts
# create some required directories
mkdir src
mkdir keys
```
