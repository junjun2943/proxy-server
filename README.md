# API Proxy Server

A lightweight Node.js proxy for forwarding API requests. Built with Express and `http-proxy-middleware`, this server is designed to route only `/api` traffic to a target service.

Part of a larger project: [Dank Memer Inventory Viewer].

## Features

- Proxies only requests starting with `/api`
- Useful for bypassing CORS issues or simplifying API access in front-end apps

## Setup

1. Clone the repo:
   ```bash
   git clone https://github.com/junjun2943/proxy-server.git
   cd proxy-server
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the server:
   ```bash
   node server.js
   ```

## Usage

Send requests to:
```
http://localhost:3000/api/<path>
```

Example:
```
http://localhost:3000/api/items
```
will forward to your target API (e.g., `https://api.gwapes.com/items`).

## License

MIT
