# pyparse 
the beginers shell language thst works anywhere
## use
this is a beginers language for shell with consise english and one-word commands that are meant to be a help.
### execution
the execution is as follows:
```shell
python pyparse.py <NAME OF THE FILE>.mtr
# to note that mtr is necesary and is the file extension
```
works in any shell and any os with a python version ahead of 3.11 

if your python is lower than python 3.11 then run
```shell
pip install tomllib
#to install all the requirements
``` 
### scripting
the scripting is very simple (the parser of the language is simple 💀).
files should start with ```#startfile.``` should end with ```#endfile.``` ,  the 
contents in between
this is done to prevent the trecherous python ```"""docstring""" ``` and the ``` /* multi line comment */```
a basic script may look like :
```mtr
#startfile.
says "hello world".
#endfile.
```
this is equavelent to a hello world program in any other language
## customization
if you are (sadly) disliking the syntax you can go to 
pyparse/code/cmdict.toml
by default , it looks like 
```toml 
# Command definitions
# {args} will be replaced by everything after the command
all = "winget install {args}"
delete  = "winget remove {args}"
update  = "winget upgrade --all"
list    = "winget list"
says    = "echo {args}"
prun    = "python {args}"
pipin  = "pip install {args}"
pipun   = "pip uninstall {args}"
pipup   = "pip install --upgrade {args}"
pipupall = "pip install --upgrade --all"
```
you can change it , add or subtract it to your harts content
and if you are on a platform that does not have powershell like linux , 
mac , etc then changt the file extension and contents in accordance to your 
os

you can change from ```runtime.ps1``` (the powershell extension) to 
```runtime.sh``` (the bash extension) or any other os's shell
for more info , i dont have any resources rn .

---

this is it for ver 0.1.0 bf proto. cya ^_____^

---

##release codes

+ *bf = before release*
+ *proto = prototype*