# Virtual Environment

## Windows

1. `python -m venv venv`
2. `\venv\Scripts\activate`

## Linux

1. `python3 -m venv venv`
2. `source venv/bin/activate`


# Poetry

`pipx install poetry` = install poetry
`pipx upgrade poetry` = upgradep oetry
`pipx uninstall poetry` = uninstall poetry

`poetry init` = initialize poetry package in the current folder
`poetry new <name>` = create a new poetry package

`python -m <module_name> -g `= For debugging
`python -m pdb -m <module_name> -g` = Python's equivalent of gdb