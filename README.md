# odt2md
Custom script to convert odt (and any supported OpenOffice Text document) into mardown. 

This script convert the text document into HTML document using `odt2html` (provided
by OpenOffice). Then convert the HTML into mardown using `pandoc`.

This script tries to fix various issues between the convertions.
* Fixes list items formating by removing `<p>` from `<li>`
* Fixes table formating by removing `<p>` from table cells
* Remove various obsolete styles `{.western}`
* Export embeded image

## Install

**Install requirements**
```
sudo apt-get install pandoc python-pandocfilters
```
I strongly recommand to install the latest pandoc from debian unstable
repo (https://packages.debian.org/sid/pandoc) or from source
(https://github.com/jgm/pandoc).

**Install script**
You may deploy the script where ever you want. To mke it accessible, I'm installing it into nautilus scripts folder as follow:
```
curl https://raw.githubusercontent.com/ikus060/odt2md/master/odt2md > "$HOME/.local/share/nautilus/scripts/odt2md"
chmod +x "$HOME/.local/share/nautilus/scripts/odt2md"
```

## Usage
```
odt2md "My file.odt"
```
This will output a file named `My file.md`
