# The Shell

### Example Debug Output

```
[chadd@cs-vm CS460_Shell]$ bin/main -d
21364> ls
command: ls
	arguments: none
	redirection:
		stdin: none
		stdout: none
	pipe: none
background: no
21364> cat hint.txt > newFile.txt
command: cat
	arguments: hint.txt
	redirection:
		stdin: none
		stdout: newFile.txt
	pipe: none
background: no
21364> cat hint.txt newFile.txt | grep fun &
command: cat
	arguments: hint.txt newFile.txt
	redirection:
		stdin: none
		stdout: PIPE
	pipe: YES
command: grep
	arguments: fun
	redirection:
		stdin: PIPE
		stdout: none
	pipe: none
background: YES
21364>  ls ; echo hi
command: ls
	arguments: none
	redirection:
		stdin: none
		stdout: none
	pipe: none
background: no
command: echo
	arguments: hi 
	redirection:
		stdin: none
		stdout: none
	pipe: none
background: no
21364> exit
[chadd@cs-vm CS460_Shell]$
```
