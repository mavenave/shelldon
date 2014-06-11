Shelldon
========

Python-wrapper of Bash (whut)
-----------------------------

###Table of Content
- [Introduction](#intro)
- [Usage](#usage)
- [License](#license)
- [Support](#support)

###Introduction<a name='intro'></a>
Whuttttt. A Python-wrapper for Bash? You know how you want to sometimes make some shell commands from Python? And then you go for:

```python
import subprocess
  
# Normally you do this from a Python script
subprocess.call(['git', 'add', '--all']
```

I find that way, way too much to type. Also, why put it into a form of a list?

Why can't we just write `subprocess.call('git add --all')`?

###Usage<a name='usage'></a>
**Normal script use:**
```python
import shelldon

shelldon.call('git add --all') # So simple isn't it?!
```

**Or, if you want to have multiple commands bundled together:**
```python
shelldon.call("""
              git add --all
              git commit -m 'Initial commit'
              git push origin master
              """)
```

**Terminal use:**
```python
>> import shelldon
>> shelldon.term()
~$ >> ls
Desktop         Programs
Documents       Public
Downloads
Music
Pictures
~$ >> cd Desktop
~/Desktop$ >> quit # Use this command to quit shelldon's terminal
>> print 'yay to using shell in Python!' # Back to Python interpreter
```


###License<a name='license'></a>
The following code is released under the MIT license. See above for it.

###Support<a name='support'></a>
If you have any questions/concerns, please feel free to contact me.
My email address is guanhao3797@gmail.com

**Will update README once project is more substantial.**
