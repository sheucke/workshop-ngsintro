# workshop-ngsintro [![gh-actions-build-status](https://github.com/nbisweden/workshop-ngsintro/workflows/build/badge.svg)](https://github.com/nbisweden/workshop-ngsintro/actions?workflow=build)

This repo contains the course material for NBIS workshop **Introduction to Bioinformatics using NGS data**. The rendered view of this repo is available [here](https://nbisweden.github.io/workshop-ngsintro/).

## Contributing

To add or update contents of this repo (for collaborators), first clone the repo.

```
git clone https://github.com/nbisweden/workshop-ngsintro.git
```

Make changes/updates as needed. Add the changed files. Commit it. Then push the repo back.

```
git add .
git commit -m "I did this and that"
git push origin
```

If you are not added as a collaborator, first fork this repo to your account, then clone it locally, make changes, commit, push to your repo, then submit a pull request to this repo.

:exclamation: When updating repo for a new course, change `output_dir: XXXX` in `_site.yml` as the first thing, so that old rendered files are not overwritten.

:exclamation: Do not push any rendered .html files or intermediates.

## Repo organisation

The source material is located on the *master* branch (default). The rendered material is located on the *gh-pages* branch. For most part, one only needs to update content in master. Changes pushed to the *master* branch is automatically rendered to the *gh-pages* branch.

:exclamation: The first build can take around 30-40 mins depending on the number of R packages (listed in **_site.yml**). Subsequent builds take about 2-3 minutes since caching is enabled. Caches are removed after 7 days of last access. A push after that will require a full rebuild.

For more details about repo organisation, updating and modifying this repo, check out the [template repo](https://github.com/royfrancis/workshop-template-rmd-ga).

## Test scripts

This is regarding the directory **scripts**. This directory contains shell scripts for reseq (variant-calling) and rnaseq parts of the workshop. These are intended to be run on UPPMAX. Further instructions on using them are available within the scripts.

The contents of these scripts should use identical steps and tools as the student would use in the lab. The aim of these scripts is to execute them on UPPMAX before the course. This should provide insight into broken links, broken tools, tool incompatibilities, core usage, ram usage and total space used.

*The scripts directory is not used in this repo, tutorial or the website. It's just here as a backup.*

---

**2020** NBIS • SciLifeLab
