# DevContainer for Playwright TypeScript

This project includes a VS Code DevContainer configuration for consistent development environment.

## Quick Start with DevContainer

### Prerequisites

- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
- [VS Code](https://code.visualstudio.com/)
- [Dev Containers Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

### Setup Steps

1. **Clone repository**:

   ```bash
   git clone <repository-url>
   cd Playwright_Typescript
   ```

2. **Open in VS Code**:

   ```bash
   code .
   ```

3. **Reopen in Container**:

   - VS Code sẽ detect DevContainer config
   - Click "Reopen in Container" notification
   - Hoặc `Ctrl+Shift+P` → "Dev Containers: Reopen in Container"

4. **Wait for setup** (tự động):

   - Container được build
   - Extensions được cài đặt
   - Dependencies được install (`npm install`)
   - Playwright browsers được download

5. **Start testing**:
   ```bash
   npm run test:ui     # Playwright UI Mode
   npm run test:smoke  # Run smoke tests
   ```

## DevContainer Benefits

**Pre-configured Environment**: All tools, extensions, browsers ready  
**Consistent Setup**: Same environment for all team members  
**Zero Config**: No manual installation needed  
**VS Code Integration**: Debugging, IntelliSense, extensions work seamlessly  
**Port Forwarding**: Access UI Mode and reports directly  
**Git Integration**: Full Git support inside container

## Available Ports

- **9323**: Playwright UI Mode

- **3000**: Application server (if needed)

## Pre-installed Extensions

- Playwright Test Runner
- TypeScript support
- ESLint & Prettier
- Markdown support
- JSON tools

## Usage Tips

- **Terminal**: Use VS Code integrated terminal (runs inside container)
- **Files**: Edit files normally in VS Code
- **Debugging**: Set breakpoints and debug tests directly
- **Extensions**: All extensions work inside container
- **Port Access**: Click on forwarded ports in VS Code status bar

## Rebuilding Container

If you need to rebuild (after config changes):

```
Ctrl+Shift+P → "Dev Containers: Rebuild Container"
```
