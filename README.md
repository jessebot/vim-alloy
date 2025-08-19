# vim-alloy

This plugin adds support for syntax higlighting Grafana Alloy configuration
syntax files.

This is a fork of [grafana/vim-alloy](https://github.com/grafana/vim-alloy) to add some more syntax matches (`alloyBlockBrace`, `alloyParentheses`, `alloyBrackets`, `alloyOperator`, `alloyPeriod`, `alloyAttribute`) to use for highlighting. It also avoids doing any actual linking of highlights in the syntax file. The whole thing is just syntax.

<img width="450" height="245" alt="Example screenshot of the syntax highlighting" src="https://github.com/user-attachments/assets/bcaf55ea-aea4-459b-b091-9e0c7b547d5c" />

I use [spacechalk.nvim](https://github.com/space-chalk/spacechalk.nvim), but here's the highlights I used there for the above screenshot:

```vim
hi def link alloyString     String
hi def link alloyEscape     Special
hi def link alloyInt        Number
hi def link alloyFloat      Number
hi def link alloyConstant   Constant
hi def link alloyComment    Comment
hi def link alloyTodo       Todo

highlight alloyBlockName    guifg=#6DF2E5 guibg=#323232
highlight alloyBlockLabel   guifg=#C1FF87 cterm=italic gui=italic
highlight alloyBlockBrace   guifg=#f289f9
highlight alloyParentheses  guifg=#7aa2f7
highlight alloyBrackets     guifg=#ff8d87
highlight alloyOperator     guifg=#f7fb53
highlight alloyPeriod       guifg=#d092fc
highlight alloyAttribute    guifg=#5cc9fd
```
