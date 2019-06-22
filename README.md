##  Project's name

Description of the project...

##  Organization of the Files

The project has the following structure (some could not apply for a particular task):

  * **_CODES**: Contains all the programming codes used in the project.
  * **_DATA**:  Has the data used throughout the development of the project.
  * **_GRAPHS**: Comprehends all the charts elaborated in the undertaking.
  * **_RESOURCES**: Include some relevant files that were used during the construction of the project.
  * **_TEXTS**: Consists of all the analyses and reports related to the project.

---

##  Some useful commands

### Command-line commands

The following statements can be useful while you are working on a project:

On Windows:

* `del /s /q .gitkeep`: It removes all the .gitignore files within the project; `/s disables` disables the command-line prompting and `/q` deletes the file from all subfolders.
* `copy *.csv consolidated_CSVs.csv`: Merge all the `CSV` files in the current directory into the `consolidated_CSVs.csv` file.  It is a way to promptly merge files!
* `mklink \H <link-file> <source-file>`: Creates a hard link of the source-file.
* `grep -v '^#' <filename> > <newfilename>`: Removes all the lines that start with the character `#`.  The `-v` tag shows all the lines that does not start with the specified regular expression. Note that you cannot overwrite the file because `grep` does not allow it, however, you can use `sed -i '/^#/ d' <filename>`.
* `dir /b/s <pattern>`: Recursively finds all the files (througout all the subfolders) that match the pattern in the current directory (e.g., if pattern is C:\*.pdf, it will print out all the pdf files in the C unit).
* `cat <filename>`: Shows the contents of the filename.
* `start .`: Opens the current directory.
* `clip < <file>`: Copy the contents of `file` to the clipboard.
* `tree /A /F | more`: Shows the file tree structure of the current directory by parts (i.e., asks input from user to continue).
* `head <regular expression> -n 2`: Displays the first 2 lines of the files with filenames that follows the given `regular expression`.

On Linux:

* `find . -name "*.gitkeep" -type f -delete`: It removes all the .gitignore files within the project.
* `ln <source-file> <link-file>`: Creates a hard link of the source-file.
* `cat <filename>`: Shows the contents of the filename.
* `pdftk <pdf-file> output <password-protected-pdf-file> userpw <password>`: Adds a password to the `pdf-file`.  You must have had to install `pdftk` (`sudo apt-get install pdftk`).  N.B.: `pdf-file` should be different to `password-protected-pdf-file`.

### Git

* In order to pull all the new files under tracking out you can use `git ls-files --others --exclude-standard`.
* You can use `git reset --hard HEAD` so as to go back to the last commit, while you can use `git checkout HEAD -- <file>` in order to go back to the previous state of file.
* With the aim to show the differences by word, you can use `git diff --color-words`.
* You may get all the files under tracking with `git ls-tree -r master --name-only`.
* In case you have amended in your local repository, and you want to push to a remote one, you can force the push using `git push -f origin master`.
* Whether you want to add a command-line shortcut to a common git command, you can use `git config --global alias.<shortcut> "commands (do not include the word git)"`; It adds a new entry in the `~/.gitconfig file` (you can know where it is located with `git config --list --show-origin`).  Thereon, you can call it with `git <shortcut>`.  You may want to consider the following shortcuts:
    - `git config --global alias.lf "ls-files --others --exclude-standard"`
    - `git config --global alias.lt "ls-tree -r master --name-only"`
    - `git config --global alias.wdiff "diff --color-words"`
    - `git config --global alias.pf "push -f origin master"`

