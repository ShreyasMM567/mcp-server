# MCP Server

A Node.js server built with the Model Context Protocol (MCP) SDK, providing a simple user management API and tools for generating and managing user data.

## Features
- List all users
- Get details for a specific user
- Create a new user
- Generate a random user with fake data
- Generate a fake user based on a given name

## Project Structure
```
├── src/
│   ├── server.ts         # Main server logic
│   └── data/
│       └── users.json    # User data storage (JSON)
├── package.json          # Project metadata and scripts
├── tsconfig.json         # TypeScript configuration
├── .gitignore            # Git ignore rules
```

## Getting Started

### Prerequisites
- Node.js (v18+ recommended)
- npm

### Installation
```sh
git clone https://github.com/ShreyasMM567/mcp-server.git
cd mcp-server
npm install
```

### Running the Server
- **Development:**
  ```sh
  npm run server:dev
  ```
- **Build:**
  ```sh
  npm run server:build
  ```

## API Overview

### Resources
- **GET users**: Returns all users from `users.json`.
- **GET user-details**: Returns details for a specific user by ID.

### Tools
- **create-user**: Create a new user (name, email, address, phone required).
- **create-random-user**: Generate and add a random user with fake data.

### Prompts
- **generate-fake-user**: Generate a fake user based on a given name.

## Data Format
User objects in `src/data/users.json`:
```json
{
  "id": 1,
  "name": "Alice Thompson",
  "email": "alice.thompson@example.com",
  "address": "123 Maple Street, Seattle, WA 98101",
  "phone": "+1-206-555-0134"
}
```

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a pull request

## License
ISC

---

For more information, see the [MCP SDK documentation](https://www.npmjs.com/package/@modelcontextprotocol/sdk). 
