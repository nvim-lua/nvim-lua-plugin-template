# nvim-lua-plugin-template

This repository is a template for Neovim plugins written in Lua.

The intention is that you use this template to create a new repository where you then adapt this readme and add your plugin code.
The template includes the following:

- GitHub workflows to run linters and tests
- Minimal test setup
- EditorConfig
- A .luacheckrc


To get started writing a Lua plugin, I recommend reading the [nvim-lua-guide][nvim-lua-guide].

## Scope

Anything that the majority of plugin authors will want to have is in scope of
this starter template. Anything that is controversial is out-of-scope.


## Template License

The template itself is licensed under the [MIT license](https://en.wikipedia.org/wiki/MIT_License).
The template doesn't include a LICENSE file. You should add one after creating your repository.

---


The remainder of the README is text that can be preserved in your plugin:

---


## Development

### Run tests


Running tests requires [plenary.nvim][plenary] to be checked out in the parent directory of *this* repository.
You can then run:

```bash
nvim --headless --noplugin -u tests/minimal.vim -c "PlenaryBustedDirectory tests/ {minimal_init = 'tests/minimal.vim'}"
```

Or if you want to run a single test file:

```bash
nvim --headless --noplugin -u tests/minimal.vim -c "PlenaryBustedDirectory tests/path_to_file.lua {minimal_init = 'tests/minimal.vim'}"
```


[nvim-lua-guide]: https://github.com/nanotee/nvim-lua-guide
[plenary]: https://github.com/nvim-lua/plenary.nvim
