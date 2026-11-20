# STEP 1

- Download [https://www.tug.org/mactex/](https://www.tug.org/mactex/mactex-download.html)
- Download https://www.texstudio.org

# STEP 2

Run the following command in terminal:
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

# STEP 3

Run the following command in terminal:
```
brew install latexdiff
```

# STEP 4

Create 2 folders:
- 1 folder with all the original submitted files ("old")
- 1 folder with all the revised files ("new")

# STEP 5

- Comment out Mark's word count command from the old and new main.tex

# STEP 6

- Compile original main.tex in TeXstudio
- Compile revised main.tex in TeXstudio

# STEP 7

Run in terminal:
```
latexdiff-so old/main.tex new/main.tex --flatten > diff.tex
```

# STEP 8

Compile the diff.tex

# Voilà!
