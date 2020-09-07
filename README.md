# hlnext.vim

> Vim global plugin for highlighting matches

This plugin is pushed as a personal GitHub repo to better manage the plugin indepedently of vim configs.

### Original links
* From Damien Conway's ['More Instantly Better Vim' OSCON 2013 talk](https://www.youtube.com/watch?v=aHm36-na4-4)
* [Tarball](http://is.gd/IBV2013)
* [Github repo](https://github.com/thoughtstream/Damian-Conway-s-Vim-Setup)
* [hlnext.vim](https://github.com/thoughtstream/Damian-Conway-s-Vim-Setup/blob/master/plugin/hlnext.vim)

## Description

After highlighting search results, shows the search result
that is found at the cursor in a different color.  Using N or n
to jump forward or backward will update the result at the
cursor to be newly highlighted.

Highlighting the next search result is done via the HLNext()
function.  In order to remove search highlighting it is
recommended to use a mapping similar to the following:

```vim
nmap <silent> <BS> :call HLNextOff() <BAR> :nohlsearch<CR>
```

If using documap.vim:

```vim
nmap <silent> <BS> [Cancel highlighting] :call HLNextOff() <BAR> :nohlsearch<CR>
```

If using documap.vim and either visualguide.vim or visualsmartia.vim

```vim
nmap <silent> <BS> [Cancel highlighting] :call HLNextOff() <BAR> :nohlsearch <BAR> :call VG_Show_CursorColumn('off')<CR>
```

## Settings

Set custom highlight colors with the following in your vimrc:

```vim
highlight default HLNext ctermfg=white ctermbg=red cterm=bold
```

## Alternatives

[vim-searchlight](https://github.com/PeterRincker/vim-searchlight/), [vim-searchhi](https://github.com/qxxxb/vim-searchhi), and [vim-searchant](https://github.com/timakro/vim-searchant) are all well-maintained and feature-full.

I am most familiar with Damain Conway's hlnext and the highlighting style, and decided to stick with it.


## Meta

* Last change:      Mon Sep  7 14:09:06 CDT 2020
* Maintainer:       [Happy-Dude](https://github.com/happy-dude)
* Original author:  [Damian Conway](https://github.com/thoughtstream)

### License

This file is placed in the public domain.

