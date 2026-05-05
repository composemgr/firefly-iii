## 👋 Welcome to firefly-iii 🚀

Personal finances manager with reporting and budgeting

## 📋 Description

Personal finances manager with reporting and budgeting

## 🚀 Services

- **firefly-iii**: fireflyiii/core:latest

### Infrastructure Components

- **firefly-iii-db**: Mariadb database


## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/firefly-iii/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/firefly-iii" ~/.local/srv/docker/firefly-iii
cd ~/.local/srv/docker/firefly-iii
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install firefly-iii
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
APP_SECRET_KEY=changeme_secret_key_32_characters_long
DB_CREATE_DATABASE_NAME=firefly
DB_USER_NAME=firefly
DB_USER_PASS=changeme_db_password
EMAIL_SERVER_HOST=172.17.0.1
EMAIL_SERVER_PORT=587
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:8080

## 📂 Volumes

- `./volumes/data/firefly-iii` - Data storage
- `./volumes/data/db/mariadb/firefly-iii` - Data storage

## 🔐 Security

- Change all default passwords before deploying to production
- Use strong secrets for all authentication tokens
- Configure HTTPS using a reverse proxy (nginx, traefik, caddy)
- Regularly update Docker images for security patches
- Backup your data regularly

## 🔍 Logging

```shell
docker compose logs -f firefly-iii
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
