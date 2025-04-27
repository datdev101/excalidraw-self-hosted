# excalidraw-self-hosted

Self-hosted deployment of [Excalidraw](https://excalidraw.com/) — a virtual whiteboard for sketching hand-drawn-like diagrams.

## Features

- **Frontend**: Excalidraw interface
- **Backend**: Excalidraw storage server
- **Docker Compose**: Easy setup with a single command

## Project Structure

```
├── frontend/        # Excalidraw frontend (UI)
├── storage-backend/ # Excalidraw backend (file storage server)
├── compose.yml      # Docker Compose file to run both services
└── .gitmodules      # Git submodules configuration
```

## Setup

1. **Clone the repo:**

   ```bash
   git clone --recurse-submodules https://github.com/datdev101/excalidraw-self-hosted.git
   cd excalidraw-self-hosted
   ```

2. **Run the services using Docker Compose:**

   ```bash
   docker compose up
   ```

3. Access Excalidraw at [http://localhost:3000](http://localhost:3000).

## Requirements

- Docker
- Docker Compose
- Git (with submodules support)

## Notes

- Ensure ports `3000` (frontend) and `5001` (backend) are available.
- You can modify `compose.yml` to customize port mapping or environment settings.

## License

This project follows the [Excalidraw license](https://github.com/excalidraw/excalidraw#license).
