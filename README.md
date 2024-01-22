
# Workshop: Introduction to Databases

_[UC Davis DataLab](https://datalab.ucdavis.edu/)_  
_Spring 2024_  
_Instructor: Elise Hellwig <<echellwig@ucdavis.edu>>_  
_Maintainer: Elise Hellwig <<echellwig@ucdavis.edu>>_

* [Reader](https://ucdavisdatalab.github.io/workshop_intro_to_databases/)
* [Event Page](https://datalab.ucdavis.edu/eventscalendar/YOUR_EVENT/)
* [Google Drive](https://drive.google.com/drive/folders/1eNbJfYcjpQsc6fx8FLcqWrgrrQaGfqL3)

## Description

This workshop provides a broad overview of the various technologies for storing
and organizing different collections of data. We will discuss how data structure
and data types impact your storage options, when you should use a database, and
which platforms you might consider for your research.  This workshop is a
general lecture with case studies and Q&A (no laptops necessary). This workshop
is a prerequisite for DataLab's "Getting started with SQL for querying
databases" workshop and part of the Research Computing micro-credential.

### Learning Goals

By the end of this workshop, learners should be able to:

* Describe different data set structures

* Compare and contrast different data storage platforms

* Explain the differences between SQL and noSQL databases

* Explain the components of an Entity Relationship Diagram (ERD)

* Define relational keys

* Identify appropriate data storage solutions based on the structure of a 
  research data set


## Contributing

The course reader is a live webpage, hosted through GitHub, where you can enter
curriculum content and post it to a public-facing site for learners.

To make alterations to the reader:
	  
1.  Check in with the reader's current maintainer and notify them about your 
    intended changes. Maintainers might ask you to open an issue, use pull 
    requests, tag your commits with versions, etc.

2.  Run `git pull`, or if it's your first time contributing, see
    [Setup](#setup).

3.  Edit an existing chapter file or create a new one. Chapter files are R
    Markdown files (`.Rmd`) at the top level of the repo. Enter your text,
    code, and other information directly into the file. Make sure your file:

    - Follows the naming scheme `##_topic-of-chapter.Rmd` (the only exception
      is `index.Rmd`, which contains the reader's front page).
    - Begins with a first-level header (like `# This`). This will be the title
      of your chapter. Subsequent section headers should be second-level
      headers (like `## This`) or below.
    - Uses caching for resource-intensive code (see [Caching](#caching)).

    Put any supporting resources in `data/` or `img/`. For large files, see
    [Large Files](#large-files). You do not need to
    add resources generated by your R code (such as plots). The knit step saves
    these in `docs/` automatically.

4.  Run `knit.R` to regenerate the HTML files in the `docs/`. You can do this
    in the shell with `./knit.R` or in R with `source("knit.R")`.

5.  When you're finished, `git add`:
    - Any files you added or edited directly, including in `data/` and `img/`
    - `docs/` (all of it)
    - `_bookdown_files/` (contains the **knitr** cache)
<!--
    - `.gitattributes` (contains the Git LFS file list)
-->

    Then `git commit` and `git push`. The live web page will update
    automatically after 1-10 minutes.


<!--
### Large Files

If you want to include a large file (say over 1 MB), you should use git LFS.
You can register a large file with git LFS with the shell command:

```sh
git lfs track YOUR_FILE
```

This command updates the `.gitattributes` file at the top level of the repo. To
make sure the change is saved, you also need to run:

```sh
git add .gitattributes
```

Now that your large is registered with git LFS, you can add, commit, and push
the file with git the same way you would any other file, and git LFS will
automatically intercede as needed.

GitHub provides 1 GB of storage and 1 GB of monthly bandwidth free per repo for
large files. If your large file is more than 50 MB, check with the other
contributors before adding it.
-->

### Github Actions

GitHub Actions can be set up to automatically render your reader when you push 
new content to a repo. If you would like to use this function, download the 
materials in [datalab-dev/utilities/render_bookdown_site][render-site] and 
follow the instructions there.

[render-site]: https://github.com/datalab-dev/utilities/tree/main/render_bookdown_site

## Setup


<!--
### Git LFS

This repo uses [Git Large File Storage][git-lfs] (git LFS) for large files. If
you don't have git LFS installed, [download it][git-lfs] and run the installer.
Then in the shell (in any directory), run:

```sh
git lfs install
```

Then your one-time setup of git LFS is done. Next, clone this repo with `git
clone`. The large files will be downloaded automatically with the rest of the
repo.

[git-lfs]: https://git-lfs.github.com/
-->


[Back to Top](#top)
