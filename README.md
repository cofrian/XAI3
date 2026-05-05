# XAI: Model-agnostic methods — Exercise 5: Partial Dependency Plot (PDP)

Authors: Luis Trigueros Espada, Fernando Martínez Gómez, Sergio Ortiz Montesinos

Project contents
- `XAI3_PDP.Rmd` — R Markdown source for the exercise
- `XAI3_PDP.html` — Rendered HTML report
- `XAI3_memoria_profesional.tex` — LaTeX document
- `data/` — datasets (`day.csv`, `kc_house_data.csv`)
- `figures/` — generated figures
- `report/` — place your final PDF/Word report here (required)

Exercise summary

This repository contains the work for "XAI: Model-agnostic methods — Exercise 5: Partial Dependency Plot (PDP)". The tasks performed are:

1) One-dimensional PDP for predicting bike rentals (`cnt`) using a Random Forest approximation. Features analyzed: days since 2011, temperature, humidity and wind speed.
2) Two-dimensional PDP (humidity vs temperature) to visualize interaction effects and density of the inputs. A random sample of the data is used to reduce computation and plotting cost.
3) PDP analysis for house prices using `kc_house_data.csv` with a Random Forest approximation and features: bedrooms, bathrooms, sqft_living, sqft_lot, floors, yr_built.

Report

Place the final report (PDF or Word) with answers and comments in the `report/` folder. The instructor will evaluate the report content.

Reproducibility

Suggested R environment and steps to reproduce the analysis:

1. Install the required R packages (example):

   install.packages(c("randomForest", "pdp", "ggplot2", "dplyr", "readr"))

2. Knit the R Markdown file:

   - Open `XAI3_PDP.Rmd` in RStudio and click "Knit" to produce `XAI3_PDP.html`.
   - Or run in R: `rmarkdown::render("XAI3_PDP.Rmd")`

Git & version control

This project uses `git` for version control. The repository is organized with two branches as required:

- `main` — primary branch with the final code and report.
- `backup` — secondary branch containing an additional checkpoint commit.

Commit history and messages

Commits include descriptive English messages explaining the changes (initialization, adding analysis files, adding README, creating backup branch). Multiple commits were created to show the development process and explanations.

How to publish to GitHub (example commands)

1. Create a new, empty repository on GitHub (do not create README there).
2. On your local machine, run these commands from the project root:

```
git init
git add .
git commit -m "Initial commit: add project files and data"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main

# Create and push the backup branch
git checkout -b backup
git commit --allow-empty -m "Checkpoint: backup branch created"
git push -u origin backup
```

Replace `<your-username>` and `<repo-name>` with your GitHub username and chosen repository name. If you use the GitHub CLI you can create and push with:

```
gh repo create <your-username>/<repo-name> --public --source=. --remote=origin
git push -u origin main
git checkout -b backup
git commit --allow-empty -m "Checkpoint: backup branch created"
git push -u origin backup
```

Notes and academic requirements

- The final repository link is the deliverable for the assignment. Ensure the `report/` folder contains the final PDF or Word file with comments and answers.
- All commit messages must be in English and descriptive.

License

This repository contains student coursework. Check with your instructor for licensing and sharing permissions.
