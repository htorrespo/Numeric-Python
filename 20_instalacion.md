<!--
https://link-springer-com.ezproxy.unal.edu.co/chapter/10.1007/978-1-4842-0553-2_20
-->

# Instalacion

This Appendix covers the installation and setup of a Python environment for scientific computing on commonly used platforms. As discussed in  Chapter 1, the scientific computing environment for Python is not a single product, but rather a diverse ecosystem of packages and libraries, and there are numerous possible ways to install and configure a Python environment on any given platform. Python itself is rather easy to install,1 and on many operating systems it is even preinstalled. All pure Python libraries that are hosted on the Python Package Index2 are also easily installed, for example, using pip and a command such as pip install PACKAGE, where PACKAGE is the name of the package to install. The pip software then searches for the package on the Python Package Index, and downloads and installs it, if it is found. For example, to install IPython we can use:

```
$ pip install ipython
```

and to upgrade an already installed package we simply add the --upgrade flag to the pip command:

```
$ pip install --upgrade ipython
```

However, many libraries for computing with Python are not pure Python libraries, and they frequently have dependencies on system libraries written in other languages, such as C and Fortran. These dependencies cannot be handled by pip and the Python Package Index, and to build such libraries from source requires C and Fortran compilers to be installed. In other words, installing a full scientific computing software stack for Python manually can be difficult, or at least time consuming and tedious. To solve this problem, there have emerged a number of prepackaged Python environments with automated installers. The most popular environments are Continuum Analytics’s Anaconda3 and Enthought’s Canopy,4 which are both sponsored by corporations with close connections to the open-source scientific Python community, and Python(x,y),5 which is a community-maintained environment that targets Microsoft’s operating systems. These environments all have in common that they bundle the Python interpreter, the required system libraries and tools, and a large number of scientific computing-oriented Python libraries in an easy-to-install distribution. Any of these environments can readily be used to set up the software required to run the code discussed in this book, but in the following we use the Anaconda environment from Continuum Analytics. In particular, we discuss Miniconda – a lightweight version of Anaconda – and the package manager conda.
