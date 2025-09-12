# Folder Structure

```
linux-dev/
├── docker-compose.yml
├── Dockerfile
├── dotfiles/          # Optional preconfigured files (can still be mounted separately)
│   ├── .tmux.conf
│   ├── .vimrc
│   └── .zshrc
├── workspace/         # Your project files
└── home/              # Persistent container home directory
```

## Run

```bash
docker compose up -d --build
docker exec -it linux-dev zsh
```


## Deps

```
apt-get update
apt-get install -y groff-base python3-pyasn1 python3-awscrt \
python3-colorama python3-cryptography python3-dateutil \
python3-distro python3-docutils python3-jmespath \
python3-prompt-toolkit python3-ruamel.yaml python3-urllib3
dpkg --configure -a
```
