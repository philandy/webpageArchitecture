#Howto Mark
This is a quick reference for Mark.

## Syntax
Command codes open (FF) and close (00) the code in containers. In browsing view, anything inside does not get displayed.
```
{/*word* *word* {*attribute* *declaration*}.}
```
* Slash [/] is to create a container.
* Dot [.] is to declare a sentence.
* Starting a command with a space forces a comment.

## Commands
code
* Used to interface with things like scripting.

link
* Force a hyperlink.

mark
* (not required) Declares code to be Mark. Primarily used to hold meta.
* Also used to contain Mark plain around other formats such as HTML or XML.
 
object
* Creates a new empty object within the tree.
 
span
* Declares abstract spans.
 
style
* Used to change styling.

## Attributes
name
* Creates an identifier interface.

source
* Points commands to a reference.
    * References should use HTML link style.

## Problems
* Currently no way to reference command codes themselves. Potential solutions:
    * Create 2 more codes.
    * Escaping.
    * Special command.
    * Web representation.
