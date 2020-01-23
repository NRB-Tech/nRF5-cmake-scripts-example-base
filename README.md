This is the base project template for [nRF5-cmake-scripts-example](https://github.com/NRB-Tech/nRF5-cmake-scripts-example), an example/tutorial for creating a CMake project for Nordic nRF52 embedded Bluetooth System-on-Chips (SoCs).

You can clone this repository and follow the instructions at that link or on [the blog post](https://www.nrbtech.io/blog/2020/1/4/using-cmake-for-nordic-nrf52-projects) for this tutorial.

The steps to recreate this from an empty directory are:

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
