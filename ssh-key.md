# Generate and register the RSA key to server

Install ssh-copy-id
```
sudo curl -L https://raw.githubusercontent.com/beautifulcode/ssh-copy-id-for-OSX/master/install.sh | sh 
```
Generate key
```
ssh-keygen -t rsa -b 4096 
```

Copy key to server
```
ssh-copy-id -i ~/.ssh/mykey user@host
```
