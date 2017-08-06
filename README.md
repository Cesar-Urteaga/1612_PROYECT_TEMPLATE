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
* `mklink \H link-file source-file`: Creates a hard link of the source-file.
* `grep -v '^#' filename > newfilename`: Removes all the lines that start with the character `#`.  The `-v` tag shows all the lines that does not start with the specified regular expression. Note that you cannot overwrite the file because `grep` does not allow it, however, you can use `sed -i '/^#/ d' filename`.
* `cat filename`: Shows the contents of the filename.

On Linux:

* `find . -name "*.gitkeep" -type f -delete`: It removes all the .gitignore files within the project.
* `ln source-file link-file`: Creates a hard link of the source-file.
* `cat filename`: Shows the contents of the filename.
