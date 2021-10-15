# dcat

A command line catalog tool for your offline data.

## With DCat you can

* create a catalog (files index) for each desired removable media (CD/DVDs, hard/flash drives) or folder
* search for a file (name or regexp) on a single catalog or your entire collection
* browse a catalog with a nice dialog interface

## Requirements

1. ruby interpreter (no additional gems required) and common linux commands (`find`, `sort`, `pv`, and `dialog`):
   
   `apt install ruby findutils coreutils pv dialog`
2. set executable bits on file: `chmod 755 dcat`

## Usage

| action | command |
|--------|---------|
| create | `dcat <i\|index>  catalog_name   path` |
| search | `dcat <s\|search> [catalog_name] regexp` |
| browse | `dcat [catalog_name]` |
| list   | `dcat ls` |
