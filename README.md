# Folders structure

linux-dev/
├── docker-compose.yml
├── Dockerfile
├── dotfiles/          # Optional preconfigured files (can still be mounted separately)
│   ├── .tmux.conf
│   ├── .vimrc
│   └── .zshrc
└── workspace/         # Your project files
└── home/              # Persistent container home directory

# Run

`docker compose up -d --build`
`docker exec -it linux-dev zsh`
