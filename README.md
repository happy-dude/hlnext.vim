# hlnext.vim

> Vim global plugin for highlighting matches

From Damien Conway's ['More Instantly Better Vim' OSCON 2013 talk](https://www.youtube.com/watch?v=aHm36-na4-4)
[Tarball](http://is.gd/IBV2013)
[Github repo](https://github.com/thoughtstream/Damian-Conway-s-Vim-Setup)
[Plugin](https://github.com/thoughtstream/Damian-Conway-s-Vim-Setup/blob/master/plugin/hlnext.vim)

This plugin is pushed as a personal GitHub repo to better manage the plugin indepedently of vim configs.

## Description

After highlighting search results, shows the search result
that is found at the cursor in a different color.  Using N or n
to jump forward or backward will update the result at the
cursor to be newly highlighted.

Highlighting the next search result is done via the HLNext()
function.  In order to remove search highlighting it is
recommended to use a mapping similar to the following:

```vimscript
nmap <silent> <BS> :call HLNextOff() <BAR> :nohlsearch<CR>
```

If using documap.vim:

```vimscript
nmap <silent> <BS> [Cancel highlighting] :call HLNextOff() <BAR> :nohlsearch<CR>
```

If using documap.vim and either visualguide.vim or visualsmartia.vim

```vimscript
nmap <silent> <BS> [Cancel highlighting] :call HLNextOff() <BAR> :nohlsearch <BAR> :call VG_Show_CursorColumn('off')<CR>
```

## Settings

Set custom highlight colors with the following in your vimrc:

```vimscript
" Default highlighting for next match...
highlight default HLNext ctermfg=white ctermbg=red cterm=bold
```

## Alternatives

[vim-searchlight](https://github.com/PeterRincker/vim-searchlight/), [vim-searchhi](https://github.com/qxxxb/vim-searchhi), and [vim-searchant](https://github.com/timakro/vim-searchant) are all well-maintained and feature-full.

I am most familiar with Damain Conway's hlnext and the highlighting style, and decided to stick with it.


## Meta

* Last change:	Thu Dec 19 16:08:21 EST 2013
* Maintainer:	Damian Conway

### License

This file is placed in the public domain.

