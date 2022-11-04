# A List of all the CLIs that I am using

- ### `nala`
    A TUI replacement `apt` that uses mirrors and parallel downloads to be a lot better
    > Automagically replace all calls to `apt` with `nala`
    > ```bash
    > # Inside ~/.bashrc (or .zshrc)
    > apt() {
    >   command nala "$@"
    > }
    > sudo() {
    >   if ["$1" = "apt" ]; then
    >       shift
    >       command sudo nala "$@"
    >   else
    >       command sudo "$@"
    >   fi
    > }
    > ```

- ### `zsh`
    The replacement for the bash shell.

    After installing, first create the file `~/.zshenv` to set zsh to store its configs in the `.config` folder
    ```bash
    echo "ZDOTDIR=$HOME/.config/zsh" > ~/.zshenv
    ```

    Then set zsh as the default shell:
    ```bash
    chsh -s $(which zsh)
    ```

    Hopefully at some point I'll be smart enough to create a github repo and backup the configs I am making...

- ### `tar`

    Example usage:
    ```bash
    tar cvfz archive.tar.gz folder/
    ```