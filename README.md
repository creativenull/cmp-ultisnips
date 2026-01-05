# cmp-ultisnips

A simple nvim-cmp source for [ultisnips](https://github.com/SirVer/ultisnips).

## Usage

```lua
require("cmp").setup({
  snippet = {
    expand = function(args)
      vim.fn["UltiSnips#Anon"](args.body)
    end
  },
  sources = cmp.config.sources({
    { name = "ultisnips" },
  })
})
```
