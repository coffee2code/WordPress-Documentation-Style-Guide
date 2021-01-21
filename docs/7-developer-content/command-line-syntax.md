# Command-line syntax

This page explains how to format commands and their arguments in documentation. For more information about other code-related documentation, see [Code in text](), [Placeholders](), and [Code examples]().

## Command prompt

When you have to show multiple lines of command-line input, initiate each line with the dollar (`$`) prompt symbol.

Don't show the current directory path before the prompt, even if part of the instruction includes creating or changing directories. This is because the directory structure might be different for the user. However, if the general context of the command-line interface changes—such as from the local machine to a remote machine—then add an additional prompt indicator for the new context.

**Examples**  

[tip] **Recommended:**  
```shell
$ wp theme activate twentytwentyone
```  
The output is the following:

```
Success: Switched to 'Twenty Twenty-One' theme.
```  
[/tip]  

[tip] **Recommended:**  
```shell
$ pwd
/srv/www/wordpress-develop.dev
$ cat wp-cli.yml
path: src/
```  
[/tip]  

For single-line commands, the command prompt, that is the dollar symbol (`$`) is optional. However, if you have to show both multi-line and single-line commands, use the command prompt symbol for overall consistency.

Use separate code blocks for command-line instructions that include both input and output lines.

**Example**  

[tip] **Recommended:**  
```shell
$ wp cap list 'editor' | xargs wp cap add 'author'
```  
The output is the following:

```
Success: Added 24 capabilities to 'author' role.
```  
[/tip]  