# nvim/vim config

My nvim/vim configuration for django/python, react/js. Simulates similar extensions in vscode such as: prettier, linting, code completion, & other useful features. 
But ... you get all of the productivity of vim 🥷🏽

- Make sure you have your .nvim configuration sourcing .vimrc
    - In `~/.config/nvim/init.vim` enter the following:
        ```
        set runtimepath^=~/.vim runtimepath+=~/.vim/after
        let &packpath = &runtimepath
        source ~/.vimrc
        ```
- Add format on save to CocConfig
    - Run `:CocConfig`
        ```
        {
            "coc.preferences.formatOnSaveFiletypes" : ["css", "markdown", "javascript", "graphql", "html", "javascriptreact", "typescript", "typescriptreact", "python"]
        }
        ```
- Install
    - Run `:PlugInstall` with editor opened
    - Run `:CocInstall coc-pyright coc-jedi coc-prettier coc-eslint coc-tslint-plugin coc-tslint coc-tsserver coc-json coc-javascript coc-vimlsp` with editor opened
