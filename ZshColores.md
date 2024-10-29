# ZSH Color Formatting types

*Note: you can't use the same codes as bash and also can't use `echo`*

## Syntax

```zsh
%F{#00ff00}Your Text %f
```

### Breakdown of the Syntax

`%F{color} YOUR TEXT %f` Foreground/Text color
`%K{color} YOUR TEXT %k` Background color
`{#00ff00}` is the actual color part where we just put the hex value of our color.
Eg: `#ff0000` is red, `#00ff00` is green and `#0000ff` is blue
Eg: we can also write names instead of values like red
output:
![output 1](/screenshots/namecolors.png)
`Your text` replace this with whatever you like.

output:
![output 1](/screenshots/zsheg1.png)

`PS1`: it is a shell prompt string variable that defines text displayed before each command you enter.
`%n`: it is used to display the username of the logged-in user.
`%m`: it shows the hostname of the system.
`%1~`: the %1 part shows the name of the current working directory and the tilde symbol will only be displayed if you are inside your home directory.

Eg:
![%n example](/screenshots/neg.png)
![%m example](/screenshots/meg.png)
![%1~ example](/screenshots/cdeg.png)

`%j` The number of jobs currently managed by the shell.
`%L` The current value of the $SHLVL variable.
`%T` The current time in 24-hour format.
`%r` Show current time in a 12-hour format with seconds.
`%D` Show the date in "yyyy-mm-dd" format.

Eg:
![%j example](/screenshots/jobseg.png)
![%L example](/screenshots/shell.png)
![%T example](/screenshots/time.png)
![%t example](/screenshots/time12.png)
![%D example](/screenshots/date.png)

For additional styling we can wrap the text with other values like

Bold:

```zsh
PS1="%F{red}%BYour Text%b %f"
```

output:
![%B example](/screenshots/boldeg.png)

Underline:

```zsh
PS1="%F{red}%UYour Text%u %f"
```

output:
![%U example](/screenshots/underlineeg.png)

Highlight:

```zsh
PS1="%F{red}%SYour Text%s %f"
```

output:
![%S example](/screenshots/higheg.png)

If we want to add anything to the right side of the prompt then we can use

```zsh
RPROMPT="%t"
```

output: time one the right side / can use anything but in example only used time
![right prompt example](/screenshots/rpeg.png)
