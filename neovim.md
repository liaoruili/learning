# Neovim

## Install 

On Ubuntu, It is a better way to download the pre-built package from github:

```bash
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux-x86_64.tar.gz
sudo tar -C /YOURPATH -xzf nvim-linux-x86_64.tar.gz
export PATH=$PATH:/YOURPATH/nvim-linux-x86_64/bin
```

## cheat  sheet

https://neovim.io/doc/user/usr_toc.html#usr_toc.txt

| mode |      key       | function                                                                      |
|:----:|:--------------:|-------------------------------------------------------------------------------|
|  N   |       J        | Delete a line break                                                           |
|  N   |       ZZ       | Writes the file and exits                                                     |
|  N   |       zz       | Puts the cursor line at the center                                            |
|  N   |       zt       | Puts the cursor line at the top                                               |
|  N   |       zb       | Puts the cursor line at the bottom                                            |
|  N   |    w b e ge    | Word movement                                                                 |
|  N   |       %        | Matching a parenthesis                                                        |
|  N   |       7G       | Moving to a specific line(7th)                                                |
|  N   | CTRL-U  CTRL-D | **Scrolls** half a screen of text                                             |
|  N   | CTRL-E  CTRL-Y | **Scrolls** one line of text                                                  |
|  N   | CTRL-F  CTRL-B | **Scrolls** a whole screen                                                    |
|  N   |       ~        | Change case of the character under the cursor                                 |
|  N   |       I        | Start Insert mode after moving the cursor to the first non-blank in the line. |
	


### [Jumps & Bookmark](https://neovim.io/doc/user/usr_03.html#03.10)
| mode |       key       | function                                       |
|:----:|:---------------:|------------------------------------------------|
|  N   |  CTRL-O CTRL-I  | **Jumps** back and forth                       |
|  N   |       ``        | **Jumps** back and forth, between two points   |
|  N   |     :mark a     | Set a **mark** named a                         |
|  N   |      ms me      | Set a **mark**(named s or e)                   |
|  N   |       `a        | Jumps mark a                                   |
|  N   | special marks ' | The cursor position before doing a jump        |
|  N   | special marks " | The cursor position when last editing the file |
|  N   | special marks [ | Start of the last change                       |
|  N   | special marks ] | End of the last change                         |

### [Changing text](https://neovim.io/doc/user/usr_04.html#04.2)

| mode |        key        | function                                       |
|:----:|:-----------------:|------------------------------------------------|
|  N   | x stands for  dl  | delete character under the cursor              |
|  N   | X  stands for  dh | delete character left of the cursor            |
|  N   | D  stands for  d$ | delete to end of the line                      |
|  N   | C  stands for  c$ | change to end of the line                      |
|  N   | s  stands for  cl | change one character                           |
|  N   | S  stands for  cc | change a whole line                            |
|  N   |        rX         | replace the character under the cursor with it |
|  N   |         .         | repeats the last change                        |

### [Text objects](https://neovim.io/doc/user/usr_04.html#04.8)
| mode | key | function                                                                |
|:----:|:---:|-------------------------------------------------------------------------|
|  N   | das | delete a sentence, you want to delete the white  space at the same time |
|  N   | dis | delete a sentence, and the white space can remain                       |