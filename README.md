# kubexec
A super small bash command to bash exec into a kubernetes pod without the complete name.
Think of it like [stern](https://github.com/wercker/stern) but for executing into a container (and much, much more basic, just two lines of bash code).

## How to install
```bash
sudo wget https://github.com/camme/kubexec/releases/download/v0.2.0/kubexec -O /usr/local/bin/kubexec
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

If you need to run it with something else than ```bash```:

```bash
kubexec frontend sh
```
