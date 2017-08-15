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
* `mklink \H <link-file> <source-file>`: Creates a hard link of the source-file.
* `grep -v '^#' <filename> > <newfilename>`: Removes all the lines that start with the character `#`.  The `-v` tag shows all the lines that does not start with the specified regular expression. Note that you cannot overwrite the file because `grep` does not allow it, however, you can use `sed -i '/^#/ d' <filename>`.
* `cat <filename>`: Shows the contents of the filename.
* `start .`: Opens the current directory.
* `clip < <file>`: Copy the contents of `file` to the clipboard.
* `tree /A /F | more`: Shows the file tree structure of the working directory by parts (i.e., asks input from user to continue).
* `head <regular expression> -n 2`: Displays the first 2 lines of the files with filenames that follows the given `regular expression`.

On Linux:

* `find . -name "*.gitkeep" -type f -delete`: It removes all the .gitignore files within the project.
* `ln <source-file> <link-file>`: Creates a hard link of the source-file.
* `cat <filename>`: Shows the contents of the filename.
* `pdftk <pdf-file> output <password-protected-pdf-file> userpw <password>`: Adds a password to the `pdf-file`.  You must have had install `pdftk` (`sudo apt-get install pdftk`).  N.B.: `pdf-file` should be different to `password-protected-pdf-file`.

### Git

* Whether you want to add a command-line shortcut to a common git command use `git config --global alias.<shortcut> 'commands (do not include the word git)'`. So you can call it with `git <shortcut>`.
