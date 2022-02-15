# Better Digraphs
Digraphs are incredibly useful, but oftentimes hard to remember. The `h digraph-table` and `h digaph-table-mbyte` entries are helpful, but cumbersome and their usage tends to interrupt the natural flow that every nvim user aspires to. Enter better-digraphs, a plugin that improves the digraph experience in nvim by adding the contents of the `digraph-table-mbyte` to a telescope finder.

# Installation
Using vim plug
```vim
Plug protex/better-digraphs
```

# Usage
The recommended mappings for this plugin are the following:
```vim
inoremap <C-k><C-k> <Cmd>lua require'betterdigraphs'.digraphs("i")<CR>
nnoremap r<C-k><C-k> <Cmd>lua require'betterdigraphs'.digraphs("r")<CR>
```

This will allow the usage of the normal `<C-k>` in insert mode and during a single character replace, but allows you to quickly pull up the search if you can't remember the digraph you're looking for. The search will allow you to fuzzy search by either digraph shortcut (OK for ✓) or official name ("CHECK MARK" for ✓).