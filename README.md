
<!-- README.md is generated from README.Rmd. Please edit that file -->

# TDS (Transport Data Science)

This repo supports teaching of the Transport Data Science module at the
University of Leeds.

The module catalogue can be found at
[`catalogue.md`](https://github.com/ITSLeeds/TDS/blob/master/catalogue.md).
The code accompanying the course can be found in the `code` folders. To
run this code you will need R and Python installed plus various packages
and libraries. This software has been packaged-up into a docker
container to ease teaching.

See here for the the timetable, a basic visualisation of which is shown
below:

  - On the University’s system (official):
    [http://timetable.leeds.ac.uk/](http://webprod3.leeds.ac.uk/catalogue/dynmodules.asp?Y=201920&M=TRAN-5340M)
  - In .ics form:
    <https://github.com/ITSLeeds/TDS/releases/download/0.20.1/tds-timetable.ics>
  - As a .csv file:
    <https://github.com/ITSLeeds/TDS/blob/master/timetable.csv>

# References

To access references collected for this course (and contribute more if
you want), you can join the ‘tds’ Zotero group:
<https://www.zotero.org/groups/956304/tds>

# Software

For this module you need to have up-to-date versions of R and RStudio.
For guidance on setting-up your computer to run R and RStudio for
spatial data, see these links:

  - Chapter 2 of Geocomputation with R (the Prerequisites section
    contains links for installing spatial software on Mac, Linux and
    Windows): <https://geocompr.robinlovelace.net/spatial-class.html>

  - Chapter 2 of the online book *Efficient R Programming*, particularly
    sections 2.3 and 2.5, for details on R installation and
    [set-up](https://csgillespie.github.io/efficientR/set-up.html) and
    the [project management
    section](https://csgillespie.github.io/efficientR/set-up.html#project-management).

## Course locations

See the image below for the course locations and the following links:

The lectures will be in the Business School Maurice Keyworth SR (1.15):
<http://students.leeds.ac.uk/room/1-01-087-2730-01-115>

The practicals will be in the West Teaching Lab Cluster (B.16):
<http://it.leeds.ac.uk/site/custom_scripts/clusters.php>

# Issues and contributing

Any feedback or contributions to this repo are welcome. If you have a
question please open an issue here (you’ll need a GitHub account):
<https://github.com/ITSLeeds/TDS/issues>

# Data

Data for course can be accessed from the repos
[Releases](https://github.com/ITSLeeds/TDS/releases) page. You can, for
example, download and unzip the data folder in a local version of the
repo (accessed by downloading and unzipp
<https://github.com/ITSLeeds/TDS/archive/master.zip> ) with the
following R
commands:

``` r
download.file("https://github.com/ITSLeeds/TDS/releases/download/0.1/data.zip", destfile = "data.zip")
unzip("data.zip")
```

If you want to be clever you can use the piggyback package:

``` r
install.packages("piggyback")
piggyback::pb_download("data.zip")

# (This package was used to upload the data with:)
# piggyback::pb_upload(file = "data.zip")
# piggyback::pb_upload(file = "codeExamples.zip")
```

``` python
import pandas as pd
e = pd.read_csv("/mnt/27bfad9a-3474-4e61-9a43-0156ebc67d67/home/robin/ITSLeeds/TDS/sample-data/everyone.csv")
pd.DataFrame.sort_values(e, "n_coffee")
```

# Other projects

  - A book on R for Geocomputation:
    <https://github.com/Robinlovelace/geocompr>
  - A Python package for OSM data analysis:
    <https://github.com/gboeing/osmnx>

<!-- # Building the website -->

<!-- To publish the slides and other content online, the following commands were used: -->
