# Knowledge Base

## Tech Stack Compatibility Records

### Vite & Node.js Version Conflict (2026-01-08)

- **Issue**: `vite` v7.3.1 failed to run with Node.js v21.6.2.
  - Error: `Vite requires Node.js version 20.19+ or 22.12+.`
- **Root Cause**: Vite v7 dropped support for odd-numbered Node.js versions (like v21) which are often non-LTS/end-of-life.
- **Solution**: Downgraded Vite to v5.x Series.
  - Command: `npm install vite@^5.0.0`
  - Installed Version: `v5.4.21`
  - Result: Successfully resolved the startup error. Verification passed on `http://localhost:5174/`.
