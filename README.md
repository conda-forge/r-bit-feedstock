About r-bit-feedstock
=====================

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/r-bit-feedstock/blob/main/LICENSE.txt)


About r-bit
-----------

Home: http://ff.r-forge.r-project.org/

Package license: GPL-2.0-or-later

Summary: True boolean datatype (no NAs),  coercion from and to logicals, integers and integer subscripts;  fast boolean operators and fast summary statistics.  With 'bit' vectors you can store true binary booleans {FALSE,TRUE} at the  expense of 1 bit only, on a 32 bit architecture this means factor 32 less  RAM and ~ factor 32 more speed on boolean operations. Due to overhead of  R calls, actual speed gain depends on the size of the vector: expect gains  for vectors of size > 10000 elements. Even for one-time boolean operations  it can pay-off to convert to bit, the pay-off is obvious, when such  components are used more than once.  Reading from and writing to bit is approximately as fast as accessing  standard logicals - mostly due to R's time for memory allocation. The package  allows to work with pre-allocated memory for return values by calling .Call()  directly: when evaluating the speed of C-access with pre-allocated vector  memory, coping from bit to logical requires only 70% of the time for copying  from logical to logical; and copying from logical to bit comes at a  performance penalty of 150%. the package now contains further classes for  representing logical selections: 'bitwhich' for very skewed selections and  'ri' for selecting ranges of values for chunked processing. All three index  classes can be used for subsetting 'ff' objects (ff-2.1-0 and higher).

About r-bit
-----------

Home: http://ff.r-forge.r-project.org/

Package license: GPL-2.0-or-later

Summary: True boolean datatype (no NAs),  coercion from and to logicals, integers and integer subscripts;  fast boolean operators and fast summary statistics.  With 'bit' vectors you can store true binary booleans {FALSE,TRUE} at the  expense of 1 bit only, on a 32 bit architecture this means factor 32 less  RAM and ~ factor 32 more speed on boolean operations. Due to overhead of  R calls, actual speed gain depends on the size of the vector: expect gains  for vectors of size > 10000 elements. Even for one-time boolean operations  it can pay-off to convert to bit, the pay-off is obvious, when such  components are used more than once.  Reading from and writing to bit is approximately as fast as accessing  standard logicals - mostly due to R's time for memory allocation. The package  allows to work with pre-allocated memory for return values by calling .Call()  directly: when evaluating the speed of C-access with pre-allocated vector  memory, coping from bit to logical requires only 70% of the time for copying  from logical to logical; and copying from logical to bit comes at a  performance penalty of 150%. the package now contains further classes for  representing logical selections: 'bitwhich' for very skewed selections and  'ri' for selecting ranges of values for chunked processing. All three index  classes can be used for subsetting 'ff' objects (ff-2.1-0 and higher).

Current build status
====================


<table>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1003&branchName=main">
            <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-bit-feedstock?branchName=main">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>linux_64_r_base4.3</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1003&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-bit-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_r_base4.3" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_r_base4.4</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1003&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-bit-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_r_base4.4" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_aarch64_r_base4.3</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1003&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-bit-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_aarch64_r_base4.3" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_aarch64_r_base4.4</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1003&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-bit-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_aarch64_r_base4.4" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_ppc64le_r_base4.3</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1003&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-bit-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_ppc64le_r_base4.3" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_ppc64le_r_base4.4</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1003&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-bit-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_ppc64le_r_base4.4" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64_r_base4.3</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1003&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-bit-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_64_r_base4.3" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64_r_base4.4</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1003&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-bit-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_64_r_base4.4" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_arm64_r_base4.3</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1003&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-bit-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_arm64_r_base4.3" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_arm64_r_base4.4</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1003&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-bit-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_arm64_r_base4.4" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_r_base4.3</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1003&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-bit-feedstock?branchName=main&jobName=win&configuration=win%20win_64_r_base4.3" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_r_base4.4</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1003&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-bit-feedstock?branchName=main&jobName=win&configuration=win%20win_64_r_base4.4" alt="variant">
                </a>
              </td>
            </tr>
          </tbody>
        </table>
      </details>
    </td>
  </tr>
</table>

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
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `r-bit` can be installed with `conda`:

```
conda install r-bit
```

or with `mamba`:

```
mamba install r-bit
```

It is possible to list all of the versions of `r-bit` available on your platform with `conda`:

```
conda search r-bit --channel conda-forge
```

or with `mamba`:

```
mamba search r-bit --channel conda-forge
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search r-bit --channel conda-forge

# List packages depending on `r-bit`:
mamba repoquery whoneeds r-bit --channel conda-forge

# List dependencies of `r-bit`:
mamba repoquery depends r-bit --channel conda-forge
```


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [anaconda.org](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

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
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@conda-forge/r](https://github.com/orgs/conda-forge/teams/r/)

