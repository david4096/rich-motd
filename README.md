# MOTD Generator

[💻Use it now!](david4096.github.io/rich-motd/)

This simple web app allows you to create a customized Message of the Day (MOTD) with ANSI color codes. You can easily apply colors, preview them live, and copy the raw ANSI code to use in a Unix terminal.

## Features

* Input a message and apply colors using ANSI escape codes.
* Live preview of the colored output.
* Copy the raw text with ANSI escape sequences for terminal use.

## How to Use

1. Enter your text in the MOTD Input box.
2. Select the color from the dropdown.
3. Highlight text in the input box and click Apply Color.
4. Click Copy MOTD to copy the raw text with ANSI codes.


## Example of Usage

After generating your MOTD, copy the text and paste it into your terminal using the echo command:

For macOS/Linux:

```
echo -e "$(pbpaste)"   # macOS
echo -e "$(xclip -selection clipboard -o)"   # Linux
```

This will display your colored MOTD with ANSI escape codes in your terminal.

Alternatively save it to a file and then you can use:

```
echo "$(<my_motd_file)"
```

## License

MIT
