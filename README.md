# dcat

A command line catalog tool for your offline data.

## With DCat you can

* create a catalog (files index) for each desired removable media (CD/DVDs, hard/flash drives) or folder
* search for a file (name or regexp) on a single catalog or your entire collection
* browse a catalog with a nice dialog interface

## Requirements

* ruby interpreter: `apt install ruby`
* linux commands find, sort, pv, dialog: `apt install findutils coreutils pv dialog`
* set executable bits on file: `chmod 755 dcat`

## Usage

`name` is the name of the catalog

* create:  `dcat <i|index>  name   path`
* search:  `dcat <s|search> [name] regexp`
* browse:  `dcat [name]`
* list  :  `dcat ls`
