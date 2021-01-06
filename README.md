# kubexec
A super small bash command to bash exec into a kubernetes pod without the complete name

## How to install
```bash
sudo wget https://github.com/camme/kubexec/releases/download/v0.1.0/kubexec -O /usr/local/bin/kubexec
sudo chmod +x /usr/local/bin/kubexec
```

## How to use it
Just write part of the pods name:

```bash
# For a pod called frontend-draft-sjehfb-123urn
kubexec frontend-draft
# or
kubexec frontend-dra 
# or
kubexec frontend 
# or
kubexec draft-sje
```
