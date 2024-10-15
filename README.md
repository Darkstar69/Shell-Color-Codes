# Bash Shell Color Codes

##### Syntax
```
echo -e "\e[31mYOUR TEXT\e[0m"
```
output:
<p style='color:red'>YOUR TEXT</p>

Explaination:

- echo is just a built in shell command to reflect the input
- `-e` is used to allow escape sequence
- `\e[m` starting of the color where between `[`  and `m` we put color codes
    - like this `\e[32m` here 32 is the color code for green
- `\e[0m` here it represents as end of color with code 0 (reset)

```
echo -e "\e[1;32;47mYOUR TEXT\e[0m"
```
output: <span style='background-color:lightgray; color:green;'>YOUR TEXT</span>

Explanatino:
- You can use combinations for multiple outputs like I did
- Just as before we used `echo` with `-e`
- But we used `1;32;47` in color code because
    - `1` here is the ASNI code for bold charachters
    - `;` is the seperator
    - `32` for foreground green color code or text color code
    - `47` is the background light gray code

- Foreground Color Codes
    - 30 - <span style='color:black'>Black</span>
    - 31 - <span style='color:red'>Red</span>
    - 32 - <span style='color:green'>Green</span>
    - 33 - <span style='color:brown'>Brown</span>
    - 34 - <span style='color:blue'>Blue</span>
    - 35 - <span style='color:purple'>Purple</span>
    - 36 - <span style='color:cyan'>Cyan</span>
    - 37 - <span style='color:lightgray'>Light Gray</span>

- Background Color Codes
    - 40 - <span style='background-color:black'>Black</span>
    - 41 - <span style='background-color:red'>Red</span>
    - 42 - <span style='background-color:green'>Green</span>
    - 43 - <span style='background-color:brown'>Brown</span>
    - 44 - <span style='background-color:blue'>Blue</span>
    - 45 - <span style='background-color:purple'>Purple</span>
    - 46 - <span style='background-color:cyan'>Cyan</span>
    - 47 - <span style='background-color:lightgray'>Light Gray</span>

  <style>
    @keyframes blink {
      50% {
        opacity: 0;
      }
    }
  </style>

- ASNI Codes
    - 0 - Normal Characters
    - 1 - <span style='font-weight:bold'>Bold Charachters</span>
    - 4 - <span style='text-decoration:underline'>Underline Charachters</span>
    - 5 - <span style='animation: blink 1s infinite;'>Blinking Charachters</span>
    - 7 - <span style='filter:invert(1)'>Reverse video Charachters</span> (Inverse)

# Shell-Color-Codes
