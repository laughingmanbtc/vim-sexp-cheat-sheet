**INITIAL CURSOR POSITION**

![image](https://user-images.githubusercontent.com/114144822/220515886-a06a31d2-3ef6-4647-a60d-1f3c78acd15b.png)

**SELECTION**

| Command | Explanation | Example |
|:-----------:|:------------:|:------------:|
| `vaf` <br> `vif`| **Select inside of paren** (Visualize A Form) <br> * `vif` excludes edge paren | ![image](https://user-images.githubusercontent.com/114144822/220515928-ff3c3b7d-0e6a-4ed1-9e52-d9d46a1cc08b.png)
| `vaF` <br> `viF` | **Select all** <br> * `viF` excludes edge paren | ![image](https://user-images.githubusercontent.com/114144822/220515960-75dff0d7-f0bd-4a6e-b162-b1cbc57e16a6.png)
| `vas` <br> `vis` | **Select string** (Visualize A String) <br> * `vis` excludes edge double quotes; Not for single quote | ![image](https://user-images.githubusercontent.com/114144822/220516061-542231e4-e17c-4efa-a69b-96f7bdea964d.png)
| `vae` <br> `vie` | **Select element** (Visualize A Element) <br> * `vie` excludes edge spaces | ![image](https://user-images.githubusercontent.com/114144822/220516061-542231e4-e17c-4efa-a69b-96f7bdea964d.png)

**MOTION**

| Command | Explanation | Example |
|:-----------:|:------------:|:------------:|
| `(` <br> `)` | **Move to nearest paren symbol** <br> * `()[]{}` but not `<>""''` | ![image](https://user-images.githubusercontent.com/114144822/220516183-f470b286-40e8-4b0b-b532-343224a2570d.png)
| `W` <br> `B` | **Move to next/prev item** | ![image](https://user-images.githubusercontent.com/114144822/220516231-94b3e7b4-1baa-4f96-88c3-2f8ee767552d.png)
| `E` <br> `gE`| **Move to next/prev element** <br> * Similar with `W`/`B` | ![image](https://user-images.githubusercontent.com/114144822/220516344-8d116bfa-8124-4eb0-b46e-00092697fc22.png)
| `[[` <br> `]]` | **Move to top next/prev paren** <br> * Jump between each defn like `{`/`}` | ![image](https://user-images.githubusercontent.com/114144822/220516603-339b8b42-4689-4386-b02f-1186cd5279a3.png)
| `[e` <br> `]e` | **Move and select next/prev element** | ![image](https://user-images.githubusercontent.com/114144822/220516637-0ee39076-2998-40b2-bfd1-275e37864916.png)

**INDENT**

| Command | Explanation | Example |
|:-----------:|:------------:|:------------:|
| `==` <br> `=-` | **Indent current paren** <br> * `=-` indent top level | ![image](https://user-images.githubusercontent.com/114144822/220515886-a06a31d2-3ef6-4647-a60d-1f3c78acd15b.png)

**WRAPPING**

`\` is `<leader>`.

| Command | Explanation | Example |
|:-----------:|:------------:|:------------:|
| `\i` <br> `\I` | **(Wrap) nearest paren + insert mode** <br> * `\i` sends cursor to head, `\I` is to tail | ![image](https://user-images.githubusercontent.com/114144822/220517581-f9f551db-5c2a-48e1-ac32-d9bfa2dbac2e.png)
| `\[` `\]` <br> `\{` `\}` | **[Wrap] nearest paren + insert mode** <br> **{Wrap} nearest paren** | ![image](https://user-images.githubusercontent.com/114144822/220517698-515c30da-1cb7-478a-a0f7-c3b438865464.png)
| `\w` <br> `\W` | **(Wrap) nearest element + insert mode** <br> * `\w` sends cursor to head, `\W` is to tail | ![image](https://user-images.githubusercontent.com/114144822/220517791-d24ddb26-11fe-4bd9-803f-67667e88d197.png)
| `\e[` `\e]` <br> `\e{` `\e}` | **[Wrap] nearest element** <br> **{Wrap} nearest element** | ![image](https://user-images.githubusercontent.com/114144822/220517890-19747168-f25d-454d-a772-315bc2e8b175.png)
| `\@` | **Remove nearest paren symbols** | ![image](https://user-images.githubusercontent.com/114144822/220517945-66745f39-2b61-4b16-84b9-46c4e73cbbba.png)
| `\o` <br> `\O` | **Remove outer paren** <br> `\O` removes inner paren | ![image](https://user-images.githubusercontent.com/114144822/220518009-fc3e1c45-efa1-41e4-8633-cab0397641b1.png)

**LIST MANIPULATION**

| Command | Explanation | Example |
|:-----------:|:------------:|:------------:|
| `<M-k>` <br> `<M-j>` | **Swap paren with prev/next one** | ![image](https://user-images.githubusercontent.com/114144822/220518263-de88cdd2-5373-4439-8bcd-e6e05c9d4b72.png)
| `<M-h>` <br> `<M-l>` | **Swap element with prev/next one** | ![image](https://user-images.githubusercontent.com/114144822/220518390-0d02a438-f3f4-4a0f-8b4f-3ed23ef10ef7.png)
| `<M-S-k>` <br> `<M-S-j>` | **Put-out first/last paren/element to outside** (Burf) | ![image](https://user-images.githubusercontent.com/114144822/220518425-7479da54-bfe0-4fe0-8f8b-ca03630949bb.png)
| `<M-S-h>` <br> `<M-S-l>` | **Pull-in paren/element at prev/next side** (Slurp) | ![image](https://user-images.githubusercontent.com/114144822/220518463-aabe9f96-e766-46e2-91c1-c94b06935e4e.png)

**INSERTION MAPPIN

`,` is `<localleader>` which is not set by default. Needs to put `vim.g.maplocalleader=','` or `let maplocalleader=','`.

| Command | Explanation | Example |
|:-----------:|:------------:|:------------:|
| `<,h>` <br> `<,l>` | *Insert mode at the first/end of paren** | ![image](https://user-images.githubusercontent.com/114144822/220518800-9a9f6887-2b25-4301-ae59-bc69b9202152.png)

**[fireplace](https://github.com/tpope/vim-fireplace)**

| Command | Explanation | Example |
|:-----------:|:------------:|:------------:|
| `\F` | **Eval top level** | ![image](https://user-images.githubusercontent.com/114144822/220518917-5701399a-086e-4e9b-9fec-8e02ad9d45ba.png)
| `\f` | **Eval paren** | ![image](https://user-images.githubusercontent.com/114144822/220518883-e66b465e-cd16-401e-8da8-180d1d7ade1e.png)
| `\e` | **Eval element** | ![image](https://user-images.githubusercontent.com/114144822/220518945-8926b7af-a88b-48cc-82ae-58d9707c00c3.png)

You need to put below settings in `init.vim`/`init.lua` to use above commands.
```
nmap <Leader>F <Plug>FireplacePrint<Plug>(sexp_outer_top_list)``
nmap <Leader>f <Plug>FireplacePrint<Plug>(sexp_outer_list)``
nmap <Leader>e <Plug>FireplacePrint<Plug>(sexp_inner_element)``
```

**ALSO**
- [vim-sexp.txt](https://github.com/guns/vim-sexp/blob/master/doc/vim-sexp.txt): There are more defalut key bindings actually.
- [cszentkiralyi/vim-sexp-cheatsheet.md](https://gist.github.com/cszentkiralyi/a9a4e78dc746e29e0cc8)
- [avescodes/sexp-cheat-sheet](https://gist.github.com/avescodes/c724b1e0cd651d2ea69a39e4c4437ed8)
