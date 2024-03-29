# **Wrap File Colletion**


## Description 

A collection of Meson git-wrap files from repositories 
given Meson build system support by Squidfarts.


## About 

One of the major problems of multiplatform development is 
wrangling all your dependencies. This is easy on Linux 
where you can use system packages but awkward on other 
platforms. Most of those do not have a package manager 
at all. This has been worked around by having third party
package managers. They are not really a solution for end 
user deployment, because you can't tell them to install a
package manager just to use your app. On these platforms 
you must produce self-contained applications.

The traditional approach to this has been to bundle 
dependencies inside your own project. Either as prebuilt 
libraries and headers or by embedding the source code 
inside your source tree and rewriting your build system to 
build them as part of your project.

This is both tedious and error prone because it is always
done by hand. The Wrap dependency system of Meson aims to
provide an automated way to do this.
