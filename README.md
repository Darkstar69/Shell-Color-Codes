# Bash Shell Color Codes

## Syntax

```bash
echo -e "\e[31mYOUR TEXT\e[0m"
```

output: YOUR TEXT

Explaination:

- echo is just a built in shell command to reflect the input
- `-e` is used to allow escape sequence
- `\e[m` starting of the color where between `[`  and `m` we put color codes
  - like this `\e[32m` here 32 is the color code for green
- `\e[0m` here it represents as end of color with code 0 (reset)

```bash
echo -e "\e[1;32;47mYOUR TEXT\e[0m"
```

output: YOUR TEXT

Explanatino:

- You can use combinations for multiple outputs like I did
- Just as before we used `echo` with `-e`
- But we used `1;32;47` in color code because
  - `1` here is the ASNI code for bold charachters
  - `;` is the seperator
    - `32` for foreground green color code or text color code
    - `47` is the background light gray code

***
![Eample Screenshot](/screenshots/ss3.png)

***

- Foreground Color Codes
  - 30 - Black
  - 31 - Red
  - 32 - Green
  - 33 - Brown
  - 34 - Blue
  - 35 - Purple
  - 36 - Cyan
  - 37 - Light Gray

- Background Color Codes
  - 40 - Black
  - 41 - Red
  - 42 - Green
  - 43 - Brown
  - 44 - Blue
  - 45 - Purple
  - 46 - Cyan
  - 47 - Light Gray

- ASNI Codes
  - 0 - Normal Characters
  - 1 - Bold Charachters
  - 4 - Underline Charachters
  - 5 - Blinking Charachters
  - 7 - Reverse video Charachters(Inverse)

***
