![banner](./sources/images/banner.png)

**Project Description**

FindInMyNote is a simple script to find a file in your notes.

## Table Of Content

1. [Requirements](#requirements)
2. [Install](#install)
3. [Usage](#usage)
4. [Update Script](#update-script)
5. [Variable Env](#variable-env)

## Requirements

- bat
- fzf

## Install

```bash
git clone https://github.com/TheHackdes/FindInMyNote
cd FindInMyNote
chmod u+x ./install
./install
```

## Usage

1. Basic simple usage. Use the environement variable in `$HOME/.config/fimn/fimn.env`. Go to ***Variable Environement*** to check the value.

```bash
fimn
```

2. Usage with options

```bash
fimn -p /search/in/this/path/ \ # Select your new path
 -e other_editor \       # Change editor text
 -x other_extention      # Select your extention
# Exemple
fimn -p /home/user/my_notes \
 -e nano \
 -x txt
```

## Update Script

1. User the command

```bash
fimn -u
```

2. Clone the project and run install

```bash
git clone https://github.com/TheHackdes/FindInMyNote
cd FindInMyNote
chmod u+x ./install
./install
```

## Variable Env

| Variable Name | Description | Default Value |
|---|---|---|
|`FIMN_DIRECTORY`|le repertoire ou son stocker les notes|**Aucune : Obligatoire**|
|`FIMN_EDITOR`|L'editeur a utiliser|`vim`|
|`FIMN_EXTENTION`|L'extention a rechercher par default |Aucun|

## To Do

- Auto download bat and fzf
- Create man
- `FIMN_PREVIEW` : Chang preview bin
- Error with space in path
