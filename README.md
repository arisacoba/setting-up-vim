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

4. Set up `.vimrc` via [Maximum Awesome](https://github.com/square/maximum-awesome)
5. (Personal preference) Update configuration to trigger NerdTree to `,` + `n`
6. (Personal preference) Enable `colorscheme dracula`. Add this in `.vimrc`
    1. With Maximum Awesome, default plugin manager is Vundle. Add this inside `.vimrc.bundles.local`

    ```bash
    Plugin 'dracula/vim', { 'name': 'dracula' }
    ```

    b. Open `.vimrc.local` , remove the current colorscheme and add this line:

    ```bash
    let g:dracula_colorterm = 0
    let g:dracula_italic = 0
    colorscheme dracula
    ```

    c. Run `:VundleInstall`

### References

1. [How to upgrade Vim](https://apple.stackexchange.com/questions/252433/how-to-upgrade-system-default-vim)
2. [colorscheme dracula](https://draculatheme.com/vim)
