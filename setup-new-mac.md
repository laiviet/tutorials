# Installation list for new Mac


## Install common softwares
Download [Google Chrome](https://www.google.com/chrome/)

Download [Mozilla Firefox](https://www.mozilla.org/en-US//)

Download [GoTiengViet](http://www.trankynam.com/gotv/)

Download [iTerm2](https://www.iterm2.com/downloads.html)

Login to [Microsoft Office 365](https://login.microsoftonline.com/)



## Install programing software

Download [Miniconda](https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh)

Download [JDK 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)

Download [JetBrains PyCharm](https://www.jetbrains.com/pycharm/)

Download [JetBrains IntelliJ IDEA](https://www.jetbrains.com/idea/)

Download [Sublime Text](https://download.sublimetext.com/Sublime%20Text%20Build%203143.dmg)

Download [TexStudio](https://sourceforge.net/projects/texstudio/?source=typ_redirect)

Download [Matlab](https://www.mathworks.com/products/matlab.html)


## Install programming environment

Generate and setup [SSH key](https://github.com/laiviet/tutorials/blob/master/ssh-key.md)

Create alias for bash
```
alias sshuv=“ssh username@uv“
```

Install python environment
```
conda create -n py27 python=2.7
source activate py27
pip install numpy scipy scikit-learn nltk pyyaml
pip install theano tensorflow
pip install keras sklearn
```
```
conda create -n py35 python=3.5
source activate py35
pip install numpy scipy scikit-learn nltk pyyaml
pip install theano tensorflow
pip install keras sklearn
```


## Install homebrew, wget

```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew install wget --with-libressl
```
