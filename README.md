# 10oct_2

Node.js tutorial demonstrating Express.js with multiple endpoints

## Description

This is a simple Node.js tutorial project that demonstrates how to create an HTTP server using the Express.js framework with multiple endpoints.

## Prerequisites

- Node.js 14.0.0 or higher (comes bundled with npm)
- npm (Node Package Manager)

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd 10oct_2
```

2. Install dependencies:
```bash
npm install
```

Installation typically takes 1-2 minutes depending on your network speed.

## Usage

To start the server:
```bash
npm start
```

Expected output:
```
Server running on port 3000
```

The server will be accessible at `http://localhost:3000`

## API Endpoints

| Method | Path | Description | Response |
|--------|------|-------------|----------|
| GET | `/hello` | Returns a hello world greeting | "Hello world" |
| GET | `/evening` | Returns an evening greeting | "Good evening" |
| * | Any other path | Returns 404 error | "404 Not Found" |

### Testing Endpoints

Using curl:
```bash
curl http://localhost:3000/hello
# Returns: Hello world

curl http://localhost:3000/evening
# Returns: Good evening
```

Using a web browser:
- Navigate to `http://localhost:3000/hello` to see "Hello world"
- Navigate to `http://localhost:3000/evening` to see "Good evening"

## Configuration

### Custom Port

You can customize the server port by setting the `PORT` environment variable:

**Unix/Linux/macOS:**
```bash
PORT=8080 npm start
```

**Windows PowerShell:**
```powershell
$env:PORT=8080
npm start
```

**Windows Command Prompt:**
```cmd
set PORT=8080
npm start
```

## License

MIT