# Powerline 
Powerline is a statusline plugin for vim, and provides statuslines and prompts for several other applications, including zsh, bash, tmux, IPython, Awesome and Qtile.
[https://github.com/powerline/powerline](https://github.com/powerline/powerline)

![image](https://github.com/a110605/powerline-plugin/blob/master/picture/shell.png)
<p align="center">
Shell Prompt 
</p> 

![image](https://github.com/a110605/powerline-plugin/blob/master/picture/vim.png)
<p align="center">
Vim Screenshot
</p> 

## Installation
### 1. Prequisitions
```
sudo apt-get install python-pip python git
```
### 2. Download and install powerline plugin


Ubuntu version greater than 14.04 

```
# sudo apt-get install powerline
```

MacOS X

```
# git clone https://github.com/a110605/powerline-plugin
# cd powerline-plugin
# ./install.py
```

### 3. Modify .bash_profile
```
# vim ~/.bash_profile
```

Append the following code to .bash_profile  

```
function powerline_shell() {
   export PS1="$(~/powerline-shell/powerline-shell.py $? 2> /dev/null)"
}
export PROMPT_COMMAND="powerline_shell; $PROMPT_COMMAND"
```

### 4. Set terminal font
```
# git clone https://github.com/a110605/powerline-font
# cd powerline-font
# ./install.py
```

More details installation information, visit [Powerline Official Documents](https://powerline.readthedocs.io/en/latest/) 

## References
- [用Powerline美化你的Mac终端和Vim](http://www.jianshu.com/p/68ef9d2e1653)
- [Powerline：漂亮的 Vim 狀態列與 Bash Shell 命令提示字串外掛](https://blog.gtwang.org/linux/powerline-adds-powerful-statuslines-and-prompts-to-vim-and-bash/)
- [幫Mac OS X上的Terminal換上華麗的powerline命令列](http://mjj.logdown.com/posts/241370-help-terminal-on-mac-os-x-for-gorgeous-powerline-on-the-command-line)




 

 
