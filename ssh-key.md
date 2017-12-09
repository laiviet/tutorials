# Generate and register the RSA key to server

Generate key
```
ssh-keygen -t rsa -b 4096 
```

Copy ID to server
```
ssh-copy-id -i ~/.ssh/mykey user@host
```
