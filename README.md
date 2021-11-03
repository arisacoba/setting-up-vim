# Setting up Vim
> ⚠️ This set up is for macOS users

<br/>

<p align='center'>
<img src='https://user-images.githubusercontent.com/8143661/132116358-0de06d69-893a-4613-8c18-c0a68e889b9e.gif'></a>
<br>Sample screenshot</p>


### Instructions

1. Get HomeBrew
2. Run HomeBrew update

    ```bash
    brew update
    ```

3. Given you're using MacOs, you'll have Vim pre-installed. Run an update instead

    ```bash
    brew upgrade vim
    ```

4. Set up `.vimrc` via [Vim Bootstrap](https://vim-bootstrap.com/)
5. Run `:PlugInstall` after generating .vimrc
6. (Personal preference) Update configuration to trigger NerdTree to `,` + `n`
7. Show hidden files for NerdTree. Go to `.vimrc.local` and add this
    
    ```bash
    let NERDTreeShowHidden=1
    ```
8. (Personal preference) Enable `colorscheme dracula`.
    1. With Vim Bootstrap, you can select dracula 

    ```bash
    Plugin 'dracula/vim', { 'name': 'dracula' }
    ```

    b. Add this as custom config 

    ```bash
    let g:dracula_colorterm = 0
    let g:dracula_italic = 0
    colorscheme dracula
    ```

### References

1. [How to upgrade Vim](https://apple.stackexchange.com/questions/252433/how-to-upgrade-system-default-vim)
2. [colorscheme dracula](https://draculatheme.com/vim)
3. [Vim Boostrap](https://vim-bootstrap.com/)
4. [arisacoba/dotfiles](https://github.com/arisacoba/dotfiles)
