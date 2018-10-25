# Run a script as deamon
```
nohup ./yourscript.sh 0<&- &>/dev/null &
```

# Parallel

Installation from source code
```
 wget http://ftpmirror.gnu.org/parallel/parallel-20170422.tar.bz2
bzip2 -dc parallel-20170422.tar.bz2 | tar xvf -
cd parallel-20170422
./configure 
make
make install
```
Create a ``list_of_commands`` to run simotaneously

```
./program params1
./program params2
./program params3
./program params4
./program params5
```


Pooling  with 4 processes <with top command>
```
parallel -j 4 < list_of_commands ; top -u <user>
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
