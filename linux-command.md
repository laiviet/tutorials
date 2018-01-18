# Run a script as deamon
```
nohup ./yourscript.sh 0<&- &>/dev/null &
```

# Wget

Download all the files in an online directory without downloading the parent directory
```
wget -r --no-parent <URL>
```


# Screen 

Create a screen session:
```
screen -S <screen-session-name>
```

Attach session
```
screen -x <screen-session-name>
```

Detach from the attached session
```
Ctrl + A + D
```

Terminate the attached session
```
Ctrl + D
```

# Anaconda

Create new environments name "py27" with python 2.7
``` 
cd $HOME
conda create -n py27 python=2.7
```
Activate the environment when you want to use it.
```
source activate py27
```
Deactivate/change environment:

```
source deactivate py27
```
