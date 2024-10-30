About r-cbctools-feedstock
==========================

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/r-cbctools-feedstock/blob/main/LICENSE.txt)

Home: https://github.com/jhelvy/cbcTools

Package license: MIT

Summary: Design and evaluate choice-based conjoint survey experiments. Generate a variety of survey designs, including random designs, full factorial designs, orthogonal designs, D-optimal designs, and Bayesian D-efficient designs as well as designs with "no choice" options and "labeled" (also known as "alternative specific") designs. Conveniently inspect the design balance and overlap, and simulate choice data for a survey design either randomly or according to a multinomial or mixed logit utility model defined by user-provided prior parameters. Conduct a power analysis for a given survey design by estimating the same model on different subsets of the data to simulate different sample sizes. Full factorial and orthogonal designs are obtained using the 'DoE.base' package (Grömping, 2018) <doi:10.18637/jss.v085.i05>. D-optimal designs are obtained using the 'AlgDesign' package (Wheeler, 2022) <https://CRAN.R-project.org/package=AlgDesign>. Bayesian D-efficient designs are obtained using the 'idefix' package (Traets et al, 2020) <doi:10.18637/jss.v096.i03>. Choice simulation and model estimation in power analyses are handled using the 'logitr' package (Helveston, 2023) <doi:10.18637/jss.v105.i10>.

Current build status
====================


<table><tr><td>All platforms:</td>
    <td>
      <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21973&branchName=main">
        <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-cbctools-feedstock?branchName=main">
      </a>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-r--cbctools-green.svg)](https://anaconda.org/conda-forge/r-cbctools) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/r-cbctools.svg)](https://anaconda.org/conda-forge/r-cbctools) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/r-cbctools.svg)](https://anaconda.org/conda-forge/r-cbctools) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/r-cbctools.svg)](https://anaconda.org/conda-forge/r-cbctools) |

Installing r-cbctools
=====================

Installing `r-cbctools` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `r-cbctools` can be installed with `conda`:

```
conda install r-cbctools
```

or with `mamba`:

```
mamba install r-cbctools
```

It is possible to list all of the versions of `r-cbctools` available on your platform with `conda`:

```
conda search r-cbctools --channel conda-forge
```

or with `mamba`:

```
mamba search r-cbctools --channel conda-forge
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search r-cbctools --channel conda-forge

# List packages depending on `r-cbctools`:
mamba repoquery whoneeds r-cbctools --channel conda-forge

# List dependencies of `r-cbctools`:
mamba repoquery depends r-cbctools --channel conda-forge
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


Updating r-cbctools-feedstock
=============================

If you would like to improve the r-cbctools recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/r-cbctools-feedstock are
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
* [@tobiasraabe](https://github.com/tobiasraabe/)

