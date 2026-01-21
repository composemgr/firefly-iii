# Firefly-iii

A self-hosted application for managing firefly-iii.

## Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/firefly-iii/main/docker-compose.yaml" | docker compose -f - up -d
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

## Configuration

See docker-compose.yaml for environment variables and configuration options.

## Documentation

Check the official project documentation for detailed setup and usage information.
