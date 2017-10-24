# General Notes
## command line notes
  * typing 'atom .' will open the current directory in atom

## atom interface
  * when folders are green, it means they have not been added to git
  * when folders are orange they've been edited and not committed (?)

## VIM Basics (*REF:Learn enough text editor to be dangerous*)
* ESC`:q!` - global quit
* `i` - turns on *insert* modal
* ESC - returns to *normal* modal
* **Editing small files**
  * arrow keys are the simplest way to navigate around VIM
  * `0` will put you at the beginning of a line
  * `$` will put you at the end of a line
  * `:q` will quit a file
  * `:q!` will force quit a file
  * `:w` writes the file, use prior to quitting
  * `ESC u` will undo similar to `^z`
  * `source file_name` activates alias or updates BASH profile of *current* terminal. The BASH is sourced each time a new terminal is opened so `source` command is only necessary if you want to update current terminal.
  * Adding an *alias* to BASH: *the purpose of an alias is  a synonym for a command or set of commands. The main use for Bash aliases is defining shorter commands for commonly used combinations*
    * EX: `ls -hartl` - long form command to list files in *human-readable values for the sizes (e.g., 29K instead of 29592 for a 29-kilobyte file), including all of them (even hidden ones), ordered by reverse time, long form*
      1. `i` (turn on insertion mode)
      2. alias acronym=`command` (define alias/shortcut)
      3. ESC (leave insertion mode)
      4. `:w` (write the file)
      5. `:q` (quit VIM)
      6. `source file_name` (update terminal)

## Vocabulary
* **ERB**: embedded ruby - refers to files with ruby code embedded in them.
  * ex: file.html.erb = file name, content and engine type. You can use erb to generate html which default usage in Rails, because that's what browsers need to display a page.
* **MVC**: model - view - controller
  * a software architectural pattern for implementing user interfaces on computers. It divides a given application into three interconnected parts. This is done to separate internal representations of information from the ways information is presented to, and accepted from, the user
  * *models and controllers are responsible for generating HTML views* - railsgirls
  * [wikipedia](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller)
  * when setting up a ruby app -
   1. create
* **VIM** (and VI):
  * VI (vee-eye) = first text editor, dates back to the earliest days of Unix
  * VIM = Vi IMproved
  * *the most important VIM command*: ESC:q! will quit VIM
* **SSH**: *secure shell*
  * a cryptographic network protocol for operating network services securely over an unsecured network.[1] The best known example application is for remote login to computer systems by users.
  * The encryption used by SSH is intended to provide confidentiality and integrity of data over an unsecured network, such as the Internet
* **shell**: the program that supplies the command line, configured by the `.bash_profile` command in VIM.
  * NOTE: file paths that beging with a `.` are hidden in the the directory when using the normal `ls` prompt or in the graphical representation
* **BASH**: the default shell on most systems, stands for *Bourne Again SHell*
