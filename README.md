# Clippy!

Before there were LLMs, there was Clippy. He'll do his absolute best to answer your questions, just as well as any AI.

This is very stupid and quickly hacked together, so don't expect much beyond a silly joke or two.

## Installation

Clippy can be run straight from a git checkout, for the full effect install the font in the `fonts` directory first.

### macOS (tested on Tahoe 26, Apple Silicone)

Follow these steps
 
1.  Install needed libraries 
    ```bash
    brew install cairo pkgconfig gtk+3 gobject-introspection pygobject3
    ```
2. point to the installed libraries in the `.zshrc` 
    ```bash
    export GI_TYPELIB_PATH="/opt/homebrew/lib/girepository-1.0"
    export DYLD_LIBRARY_PATH="/opt/homebrew/lib"
    ```

3. Build a virtual environment f.e.
    ```bash
    uv venv
    ```
3. Run it!
    ```bash
    uv run clippy.py
    ```

For debugging, be sure to set the paths in terminal that is used pointing to the installations of the gnome-related et al. libraries. 

## Run

Just run clippy.py

If you're feeling adventurous you can bind him to a Co-pilot (or similar) key. In GNOME this can be acheived by going to Settings -> Keyboard -> View and Customise Shortcuts -> Custom Shortcuts

It is only tested on Linux and requires GTK 3.

## Roadmap

Nothing. Clippy is perfect as he is.

## Macos