# Riding the population wave

Visualises the change in countries' demographic profiles over time.

## ♻️ Use + Remix rights

![[Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0)](https://mirrors.creativecommons.org/presskit/buttons/80x15/png/by.png)

These charts, as well as the analyses that underpin them, are available under a Creative Commons Attribution 4.0 licence. This includes commercial reuse and derivates.

<!-- Do any of the data sources fall under a different licence? If so, describe the licence and which parts of the data fall under it here! if most of it does, change the above and replace LICENCE.md too -->

Data in these charts comes from:

* [UN Population Division](https://population.un.org)

**Please attribute 360info and the data sources when you use and remix these visualisations.**

## 📽 Ready-to-use graphics

Animations and image sequences ready for editing software are in the [`/out`](./out) folder.

## 🛠 Reproduce the analysis

### 💨 Quickstart: use the dev container

This project comes with a ready-to-use [dev container](https://code.visualstudio.com/docs/remote/containers) that includes everything you need to reproduce the analysis (or do a similar one of your own!), including [R](https://r-project.org) and [Quarto](https://quarto.org).

You can run the container in GitHub Codespaces without any setup:

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/360-info/report-population-power)

Or, if you have Docker installed, you can build and run the container locally:

  - Download or clone the project
  - Open it in [Visual Studio Code](https://code.visualstudio.com)
  - Run the **Remote-Containers: Reopen in Container** command

Once the container has launched (it might take a few minutes to set up the first time), you can run the analysis scripts with:

```sh
quarto render
```

Or look for the `.qmd` files to modify the analysis. (Note: the image sequence rendering in `index.qmd` throws an error that may prevent the file from being rendered normally. You can still run the code chunks manually in the codespace.)

### Manual setup

To setup a development environment manually, 

You'll need to:
- [Download and install Quarto](https://quarto.org/docs/get-started)
- [Download the install R](https://www.r-project.org)
- Satisfy the R package dependencies. In R:
  * Install the [`renv`](https://rstudio.github.io/renv) package with `install.packages("renv")`,
  * Then run `renv::restore()` to install the R package dependencies.
  * (For problems satisfying R package dependencies, refer to [Quarto's documentation on virtual environments](https://quarto.org/docs/projects/virtual-environments.html).)

Now, render the `.qmd` files to the `/out` directory with:

```sh
quarto render
```

## Help

If you find any problems with our analysis or charts, please feel free to [create an issue](https://github.com/360-info/report-population-power/issues/new)!
