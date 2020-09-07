# hlnext.vim

> Vim global plugin for highlighting matches

Pushed as a personal repo to manage the plugin indepedent of vim config and dotfiles.

### References
* Damien Conway's ['More Instantly Better Vim' OSCON 2013 talk](https://www.youtube.com/watch?v=aHm36-na4-4)
* [hlnext.vim](https://github.com/thoughtstream/Damian-Conway-s-Vim-Setup/blob/master/plugin/hlnext.vim)
* [Tarball](http://is.gd/IBV2013)
* [Github repo](https://github.com/thoughtstream/Damian-Conway-s-Vim-Setup)

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

## Alternatives

[vim-searchlight](https://github.com/PeterRincker/vim-searchlight/), [vim-searchhi](https://github.com/qxxxb/vim-searchhi), and [vim-searchant](https://github.com/timakro/vim-searchant) are feature rich and well-maintained.

I have used Damain Conway's hlnext the longest and am most familiar with it's highlighting style, and thus have stuck with it.

## Meta

* Last change:      Mon Sep  7 14:26:53 CDT 2020
* Maintainer:       [Happy-Dude](https://github.com/happy-dude)
* Original author:  [Damian Conway](https://github.com/thoughtstream)

### License

This file is placed in the public domain.

