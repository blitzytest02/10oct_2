# Node.js + Express.js Tutorial

A simple Node.js tutorial project demonstrating Express.js framework integration with multiple HTTP endpoints. This project serves as a beginner-friendly introduction to building web servers with Express.js.

## Prerequisites

Before running this project, ensure you have the following installed:

- **Node.js**: Version 14.0.0 or higher (v20.x recommended)
- **npm**: Version 6.0.0 or higher (comes bundled with Node.js)

To verify your installations:

```bash
node --version
npm --version
```

## Installation

Follow these steps to set up the project:

1. **Clone the repository:**

```bash
git clone <repository-url>
cd 10oct_2
```

2. **Install dependencies:**

```bash
npm install
```

This will install Express.js and all required dependencies. Installation typically takes 1-2 minutes depending on your network speed.

## Usage

### Starting the Server

To start the server, run:

```bash
npm start
```

**Expected Output:**

```
Server running on port 3000
```

The server will start and listen on port 3000 by default. You can now access the endpoints using a web browser or command-line tools like `curl`.

### Testing Endpoints

**Using curl:**

```bash
# Test the /hello endpoint
curl http://localhost:3000/hello

# Test the /evening endpoint
curl http://localhost:3000/evening
```

**Using a web browser:**

- Navigate to `http://localhost:3000/hello` → Displays "Hello world"
- Navigate to `http://localhost:3000/evening` → Displays "Good evening"

## API Endpoints

The server exposes the following HTTP endpoints:

| Method | Path | Response | Status Code | Description |
|--------|------|----------|-------------|-------------|
| GET | `/hello` | "Hello world" | 200 OK | Returns a simple hello world greeting |
| GET | `/evening` | "Good evening" | 200 OK | Returns a good evening greeting |
| * | (any other path) | "404 Not Found" | 404 | Handles unmatched routes with 404 error |

## Configuration

### Port Configuration

By default, the server runs on port **3000**. You can customize the port using the `PORT` environment variable:

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

## Project Structure

```
/
├── .gitignore           # Git ignore rules
├── README.md            # This file
├── package.json         # Project manifest and dependencies
├── package-lock.json    # Dependency lock file
├── server.js            # Main Express.js application
└── node_modules/        # Installed dependencies (not in version control)
```

## License

This project is licensed under the MIT License.