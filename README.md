<p align="center">
  <a href="LICENSE"><img alt="License" src="https://img.shields.io/github/license/ikus060/odt2md"></a>
  <a href="https://gitlab.com/ikus-soft/odt2md/pipelines"><img alt="Build" src="https://gitlab.com/ikus-soft/odt2md/badges/master/pipeline.svg"></a>
</p>

# odt2md

**odt2md** is a small script designed to quickly convert ODT (Open Document Text) files to Markdown text files. It utilizes the powerful `pandoc` library and `odt2html` with additional filters to generate well-formatted Markdown output.

## Features

* Fixes list item formatting by removing unnecessary <p> tags from <li> elements.
* Fixes table formatting by removing unnecessary <p> tags from table cells.
* Removes various obsolete styles (e.g., {.western}).
* Exports embedded images along with the converted Markdown file.

## Installation

### Dependencies

Before installing odt2md, make sure you have the following dependencies installed on your system:

* pandoc
* python3-pandocfilters
* unoconv
* zenity

```sh
sudo apt-get install pandoc python3-pandocfilters unoconv zenity
```

### Install as Nautilus Script

To install odt2md as a Nautilus script for easy access, follow these steps:

1. Download the script:

    ```sh
    curl https://raw.githubusercontent.com/ikus060/odt2md/master/odt2md > /usr/local/bin/odt2md
    ```

2. Make the script executable:

    ```sh
    chmod +x /usr/local/bin/odt2md
    ```

3. And create a symlink to the scripts directory in your Nautilus configuration folder:

    ```sh
    ln -s /usr/local/bin/odt2md "$HOME/.local/share/nautilus/scripts/odt2md"
    ```

## Usage

Once odt2md is installed, you can use it to convert ODT files to Markdown format. Simply open a terminal and navigate to the location of the ODT file you want to convert. Then run the following command:

```sh
odt2md "My file.odt"
```

This command will generate a Markdown file named My file.md in the same location as the original ODT file.

## Contributing

Contributions to odt2md are always welcome. If you encounter any issues or have suggestions for improvement, please feel free to [open an issue](https://github.com/ikus060/odt2md/issues/new) or submit a pull request on the [GitHub repository](https://github.com/ikus060/odt2md).

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
