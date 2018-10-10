About r-bit
===========

Home: http://ff.r-forge.r-project.org/

Package license: GPL-2

Feedstock license: BSD 3-Clause

Summary: bitmapped vectors of booleans (no NAs),  coercion from and to logicals, integers
and integer subscripts;  fast boolean operators and fast summary statistics.  With
''bit'' vectors you can store true binary booleans {FALSE,TRUE} at the  expense
of 1 bit only, on a 32 bit architecture this means factor 32 less  RAM and ~ factor
32 more speed on boolean operations. Due to overhead of  R calls, actual speed gain
depends on the size of the vector: expect gains  for vectors of size > 10000 elements.
Even for one-time boolean operations  it can pay-off to convert to bit, the pay-off
is obvious, when such  components are used more than once.  Reading from and writing
to bit is approximately as fast as accessing  standard logicals - mostly due to
R''s time for memory allocation. The package  allows to work with pre-allocated
memory for return values by calling .Call()  directly: when evaluating the speed
of C-access with pre-allocated vector  memory, coping from bit to logical requires
only 70% of the time for copying  from logical to logical; and copying from logical
to bit comes at a  performance penalty of 150%. the package now contains further
classes for  representing logical selections: ''bitwhich'' for very skewed selections
and  ''ri'' for selecting ranges of values for chunked processing. All three index  classes
can be used for subsetting ''ff'' objects (ff-2.1-0 and higher).




Current build status
====================

[![Linux](https://img.shields.io/circleci/project/github/conda-forge/r-bit-feedstock/master.svg?label=Linux)](https://circleci.com/gh/conda-forge/r-bit-feedstock)
[![OSX](https://img.shields.io/travis/conda-forge/r-bit-feedstock/master.svg?label=macOS)](https://travis-ci.org/conda-forge/r-bit-feedstock)
[![Windows](https://img.shields.io/appveyor/ci/conda-forge/r-bit-feedstock/master.svg?label=Windows)](https://ci.appveyor.com/project/conda-forge/r-bit-feedstock/branch/master)

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-r--bit-green.svg)](https://anaconda.org/conda-forge/r-bit) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/r-bit.svg)](https://anaconda.org/conda-forge/r-bit) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/r-bit.svg)](https://anaconda.org/conda-forge/r-bit) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/r-bit.svg)](https://anaconda.org/conda-forge/r-bit) |

Installing r-bit
================

Installing `r-bit` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
```

Once the `conda-forge` channel has been enabled, `r-bit` can be installed with:

```
conda install r-bit
```

It is possible to list all of the versions of `r-bit` available on your platform with:

```
conda search r-bit --channel conda-forge
```


About conda-forge
=================

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/)
and [TravisCI](https://travis-ci.org/) it is possible to build and upload installable
packages to the [conda-forge](https://anaconda.org/conda-forge)
[Anaconda-Cloud](https://anaconda.org/) channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating r-bit-feedstock
========================

If you would like to improve the r-bit recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/r-bit-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string)
   back to 0.
