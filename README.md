# dcat

A command line catalog tool for your offline data.

After trying some other tools ([CDcat](http://cdcat.sourceforge.net), [VVV](http://vvvapp.sourceforge.net), [Basenji](https://launchpad.net/basenji), [GWhere](http://www.gwhere.org), [catcli](https://github.com/deadc0de6/catcli)) I ended up writing my own with these points in mind:
- no GUI: usable everywhere especially in remote terminals
- no extra libraries needed, only mature core tools
- data stored in a compressed and open format (gzipped json)
- easy way to browse a catalog with [ncurses](https://en.wikipedia.org/wiki/Ncurses)

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
| list   | `dcat ls` |
| search | `dcat <s\|search> [catalog_name] regexp` |
| browse | `dcat [catalog_name]` |

## Screenshots

### create
![create](/sshots/create.png?raw=true "create a catalog")

### list
![list](/sshots/list.png?raw=true "list created catalogues")

### search
![search1](/sshots/search1.png?raw=true "search in catalogues")

![search2](/sshots/search2.png?raw=true "search in catalogues")

### browse
![browse1](/sshots/browse-list.png?raw=true "browse - list of catalogues")

![browse2](/sshots/browse-catalog.png?raw=true "browse a catalog")
