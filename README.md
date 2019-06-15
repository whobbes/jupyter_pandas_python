# Python and Pandas can process your data in 10 lines of code

## Abstract

Data importing, processing and visualization usually needs lots of boilerplate code and run slow. This means that exploratory data analysis is often not done or take a lot of time. In this workshop, I will teach you how Python and Pandas can process your data in 10 lines of code.

>Format: 90 minutes workshop

## Prerequisites

* Laptop
* Python 3.x
  * Pip3 - Packages manager
  * Numpy - Scientific Computing
  * Matplotlib - 2D Plotting
  * Pandas - Data Analysis
  * Jupyter - notebook server
  * (Optional) xlrd - Excel file reading

### Installation

#### Homebrew

The missing package manager for macOS

`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

#### Python

Favorite animal of the zoo

`brew install python3`

#### Python dependencies

using pip3 the nice package manager

`pip3 install -r requirements.txt`

(Optional) install `xlrd` with `pip3 install xlrd`

## Content of the session

### Basics - 45mins

Open Notebook and follow instructor in executing the code and reflecting on output.

#### Setup

#### DataFrame

#### Files I/O

#### Statistics

#### Visualisation

### Exploration - 35mins

Open Notebook, answer a few question about the dataset, create your own questions, answer them.

### Wrapping-up and next steps - 10mins

## Authors

[Sylvain Viguier](whobbes.com)

## License

MIT - see [LICENSE.md](LICENSE.md)

## References

Blooth dataset obtained via the very good intro to Pandas made by alandrex

[blooth_dataset](https://github.com/alanderex/pydata-pandas-workshop/blob/master/notebooks/1%20Reading%20and%20writing%20data%20across%20multiple%20formats.ipynb)

github metadata dataset obtained via Google BigQuery

```sql
SELECT *
FROM `bigquery-public-data.github_repos.sample_repos`
ORDER  BY watch_count DESC
LIMIT 400000
```

```sql
SELECT *
FROM `bigquery-public-data.github_repos.sample_files` AS files
INNER JOIN `bigquery-public-data.github_repos.sample_repos` AS repos
USING (repo_name)
ORDER  BY watch_count DESC
LIMIT 400000
```
