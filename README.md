# Port-MCP Stack

**Complete Docker Port Management Solution**

Deploy both Port-MCP (backend API) and Port-MCP Enforcer (web UI) with a single command.

## 🚀 Quick Start
```bash
# Clone or download docker-compose.yml
curl -O https://raw.githubusercontent.com/msw3msw/port-mcp-stack/main/docker-compose.yml

# Edit HOST_IP to match your server
nano docker-compose.yml

# Deploy both containers
docker-compose up -d
```

## 📦 What's Included

### Port-MCP (Backend API)
- 🔍 Docker port and network observability
- 📋 Port registry and policy management
- 🎯 Collision detection and reconciliation
- **Port:** 4100

### Port-MCP Enforcer (Web UI)
- 🎨 Visual container classification
- ✅ Port standardization wizard
- 📊 Compliance tracking
- 🔄 Snapshot-based rollback
- **Port:** 4200

## 🌐 Access

- **Port-MCP API:** `http://YOUR-IP:4100`
- **Port-MCP Enforcer UI:** `http://YOUR-IP:4200`

## 📖 Documentation

- [Port-MCP](https://hub.docker.com/r/msw3msw/port-mcp)
- [Port-MCP Enforcer](https://hub.docker.com/r/msw3msw/port-mcp-enforcer)

## 🎯 Port Standards

- **System:** 1-1023
- **Apps:** 1024-19999
- **Games:** 7000-9999 OR 20000-39999
- **Reserved:** 40000-45000

## ⚙️ Configuration

Edit `docker-compose.yml` and change:
- `HOST_IP` - Your Unraid/server IP address

## 📁 Volumes

Data persists in:
- `./port-mcp-data` - Port registry and policy
- `./enforcer-snapshots` - Execution history
- `./enforcer-data` - UI preferences

## 🔐 Safety

- ✅ Dry-run mode
- ✅ Manual confirmation required
- ✅ Snapshot-based rollback
- ✅ Read-only Docker socket for backend

## License

MIT
