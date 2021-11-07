# v2SimpleStyle
Simple theme for Beamer.  

<div align="right">
    <a href="./README.md">English</a> | <a href="./README_JP.md">日本語</a>
</div>
  
[View Sample.](./sample/sample.pdf)

## Command
### Change the theme color
```tex
\definecolor{themeColor}{HTML}{E03200}
```
- This sample set color `E03200`.
- If you want to other color, change color code (RGB).

### Showing citations in frame
```tex
\pagereference{\cite[???] ??????? ???????????}
```
- Display the citation at the bottom of the frame.
- See the sample (`./sample/02_sample.tex`) for details.
- This command use textpos absolute. Be careful of layout collapse!

## Necessary
- `xelatex` and `pbibtex` and `xdvipdfmx`

## Compile
```shell
make
```
- Use makefile.

## LICENSE
- MIT License
  - `from v2SimpleStyle` or `use v2SimpleStyle`?
  - If you use it for a slide theme, you don't have to write it.
