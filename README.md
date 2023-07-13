# header.nvim

**heaver.nvim is a Neovim plugin which adds brief author information and license headers to the top of the files.**

## Prerequisites

- Neovim 0.8+

## Installing

with [packer.nvim](https://github.com/wbthomason/packer.nvim)

```lua
use({ "attilarepka/header.nvim", config = function() require("header").setup() end})
```

with [lazy.nvim](https://github.com/folke/lazy.nvim)

```lua
{"attilarepka/header.nvim", config = true}
```

## Setup

The script comes with the following defaults:

```lua
{
    file_name = true,
    author = nil,
    project = nil,
    date_created = true,
    date_created_fmt = "%Y-%m-%d %H:%M:%S",
    line_separator = "------",
    copyright_text = nil,
}
```

To override the custom configuration, call:

```lua
require("header").setup({
  -- your override config
})
```

Example:

```lua
require("header").setup({
    file_name = true,
    author = "Foo",
    project = "header.nvim",
    date_created = true,
    date_created_fmt = "%Y-%m-%d %H:%M:%S",
    line_separator = "------",
    copyright_text = "Copyright 2023",
})
```

## Commands

### Adding Headers

- `:AddHeader` Adds brief copyright information

### Adding Licenses

- `:AddLicenseAGPL3` Adds **AGPL3 License**
- `:AddLicenseAPACHE` Adds **Apache License**
- `:AddLicenseBSD2` Adds **BSD2 License**
- `:AddLicenseBSD3` Adds **BSD3 License**
- `:AddLicenseCC0` Adds **CC0 License**
- `:AddLicenseGPL3` Adds **GPL3 License**
- `:AddLicenseISC` Adds **ISC License**
- `:AddLicenseMIT` Adds **MIT License**
- `:AddLicenseMPL` Adds **MPL License**
- `:AddLicenseUNLICENSE` Adds **Unlicense License**
- `:AddLicenseWTFPL` Adds **WTFPL License**
- `:AddLicenseX11` Adds **X11 License**
- `:AddLicenseZLIB` Adds **ZLIB License**

## Supported File Types

- c
- cc
- cpp
- h
- hh
- hpp
- py
- robot
- lua
- java
- js
- cs
- swift
- rb
- kt
- sc
- go
- rs
- php
- sh
- hs
- lhs
- pl
- ts
- tsx
- coffee
- groovy
- gvy
- gy
- gsh
- dart
- r

## Contributing

Open a GitHub issue or pull request.