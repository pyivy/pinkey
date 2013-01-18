# Scripts

## Nir Hide

```python
import sys
import os

u_input =  raw_input("Please enter the act:\n[H]ide or [S]how\n")
title =  raw_input("Please enter the title:\n")
u_act = u_input.lower()
if u_act == "h" or u_act == "hide":
	act = "hide"
elif u_act == "s" or u_act == "show":
	act = "show"
else:
	act = "hide"
str_command = "nircmd win %s ititle %s" % (act,title)
print str_command
os.popen(str_command)
print "done"
```