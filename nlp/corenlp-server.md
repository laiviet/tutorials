# Start a Stanford CoreNLP server

Download from [corenlp](https://stanfordnlp.github.io/CoreNLP/download.html)
```
wget http://nlp.stanford.edu/software/stanford-corenlp-full-2017-06-09.zip
unzip stanford-corenlp-full-2017-06-09.zip
cd stanford-corenlp-full-2017-06-09
```

Create the scripts
```
echo -e '#!/bin/bash \njava -mx4g -cp "*" edu.stanford.nlp.pipeline.StanfordCoreNLPServer -port 9000 -timeout 15000' > startserver.sh
chmod +x startserver.sh
```

Start the server in interactive mode
```
./startserver.sh
```

Start the server as deamon
```
nohup ./startserver.sh 0<&- &>/dev/null &
```
