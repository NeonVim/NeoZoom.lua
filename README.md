NeoZoom.lua
---


### News: A Breaking Change(ABC)

TL;DR: Using floating window instead of vim-tab to simulate "zoom-in".

---

> Wait, What? But I want to use the old one!

The old one can be found on branch `neo-zoom-original`!

---

advantages:
1. code down to 60 lines
2. no state, so no overhead (compared to the original version, see branches)
3. just one command left, `NeoZoomToggle`


```lua
use {
  'nyngwang/NeoZoom.lua',
  -- branch = 'neo-zoom-original', -- UNCOMMENT THIS, if you prefer the old one
  config = function ()
    vim.keymap.set('n', '<CR>', function ()
      vim.cmd('NeoZoomToggle')
    end, NOREF_NOERR_TRUNC)
  end
}
```

Change `<CR>` to whatever shortcut you like~


### DEMO

will be uploaded

