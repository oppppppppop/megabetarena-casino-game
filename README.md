# MegaBetArena - Web3 Casino Platform

<div align="center">

![MegaBetArena Hero Banner](./assets/images/hero-banner.jpg)

**A decentralized casino platform built on Solana blockchain, featuring multiple games, real-time betting, and transparent on-chain transactions.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Next.js](https://img.shields.io/badge/Next.js-000000?logo=next.js&logoColor=white)](https://nextjs.org/)
[![Solana](https://img.shields.io/badge/Solana-9945FF?logo=solana&logoColor=white)](https://solana.com/)

</div>

## Project Structure

```
megabetarena/
├── assets/               # Project assets and images
│   └── images/          # README and documentation images
├── backend/              # Backend API server (Express + TypeScript)
│   ├── src/
│   │   ├── config/      # Configuration files
│   │   ├── controllers/ # Request handlers
│   │   ├── middleware/  # Express middleware
│   │   ├── models/      # MongoDB models
│   │   ├── routes/      # API routes
│   │   ├── services/    # Business logic
│   │   ├── utils/       # Utility functions
│   │   ├── validators/  # Request validation
│   │   └── index.ts     # Entry point
│   └── package.json
│
├── frontend/             # Frontend application (Next.js)
│   ├── app/             # Next.js app directory
│   ├── components/       # React components
│   ├── hooks/           # Custom React hooks
│   ├── lib/             # Utility libraries
│   └── package.json
│
└── contracts/            # Solana smart contracts (Anchor)
    └── solana/          # Solana programs
        ├── programs/    # Anchor programs
        │   └── coinflip/
        ├── tests/       # Contract tests
        └── Anchor.toml
```

## Features

- 🎮 **Multiple Casino Games**: Coinflip, Slots, Dice, and more
- 🔐 **Wallet Authentication**: Secure Solana wallet-based authentication
- 💰 **On-Chain Transactions**: All bets and payouts on Solana blockchain
- 📊 **Leaderboards**: Track top players and big wins
- 🔄 **Real-Time Updates**: WebSocket support for live game updates
- 🎯 **Transparent**: All game results verifiable on-chain

## Tech Stack

### Backend
- Node.js + TypeScript
- Express.js
- MongoDB + Mongoose
- Solana Web3.js + Anchor
- Socket.io
- JWT Authentication

### Frontend
- Next.js 16
- React 19
- TypeScript
- Tailwind CSS
- shadcn/ui components

### Smart Contracts
- Solana (Anchor framework)
- Rust

## Getting Started

### Prerequisites

- Node.js 18+ and npm/pnpm
- MongoDB (local or cloud)
- Solana CLI tools (for contract deployment)
- Rust and Anchor (for contract development)

### Backend Setup

1. Navigate to backend directory:
```bash
cd backend
```

2. Install dependencies:
```bash
npm install
```

3. Copy environment variables:
```bash
cp .env.example .env
```

4. Update `.env` with your configuration

5. Run development server:
```bash
npm run dev
```

### Frontend Setup

1. Navigate to frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
pnpm install
```

3. Run development server:
```bash
pnpm dev
```

### Smart Contracts Setup

1. Navigate to contracts directory:
```bash
cd contracts/solana
```

2. Build contracts:
```bash
anchor build
```

3. Run tests:
```bash
anchor test
```

4. Deploy (to devnet):
```bash
anchor deploy
```

## Environment Variables

### Backend (.env)
- `MONGODB_URI` - MongoDB connection string
- `JWT_SECRET` - Secret key for JWT tokens
- `SOLANA_RPC_URL` - Solana RPC endpoint
- `PROGRAM_ID` - Deployed program ID
- See `backend/.env.example` for full list

## API Documentation

The backend API provides endpoints for:
- Authentication (`/api/auth`)
- Games (`/api/games`)
- Transactions (`/api/transactions`)
- Leaderboard (`/api/leaderboard`)

See `backend/README.md` for detailed API documentation.

## Development

### Running All Services

1. Start MongoDB
2. Start backend: `cd backend && npm run dev`
3. Start frontend: `cd frontend && pnpm dev`

### Testing

- Backend: `cd backend && npm test`
- Contracts: `cd contracts/solana && anchor test`

## Screenshots

<div align="center">

### Featured Games

![Coinflip Game](./assets/images/coinflip-game.jpg)
*Coinflip Game - Fast-paced coin flipping action*

![Dice Game](./assets/images/dice-game.jpg)
*Dice Game - Roll the dice and win big*

![Slots Game](./assets/images/slots-game.jpg)
*Slots Game - Classic slot machine experience*

### Additional Assets

| | | |
|---|---|---|
| ![Asset 1](./assets/1.png) | ![Asset 2](./assets/2.png) | ![Asset 3](./assets/{01749521-3182-4835-8B5D-5102C041D82A}.png) |
| ![Asset 4](./assets/{3D0B0B7C-5963-4303-8D4F-FAD120B309A8}.png) | ![Asset 5](./assets/{6EECAA16-12D5-4DD9-9E3D-B370FECF2378}.png) | ![Asset 6](./assets/{72C7AA26-695D-45D0-B0E0-8B192635E668}.png) |
| ![Asset 7](./assets/{ADABD8C1-C5A2-4EA6-B76D-CD07039712B7}.png) | ![Asset 8](./assets/{C4BA8AAD-F6B1-4C6E-B2FB-394831C9D413}.png) | ![Asset 9](./assets/{CC42964C-B601-45CE-AEA8-3CA398ED99C5}.png) |
| ![Asset 10](./assets/{E0288AD4-B38D-47EE-AB64-FFA525CCE978}.png) | | |

</div>

## Architecture

```
┌─────────────┐      ┌──────────────┐      ┌─────────────┐
│   Frontend  │──────│   Backend    │──────│  MongoDB    │
│  (Next.js)  │      │  (Express)   │      │  Database   │
└─────────────┘      └──────────────┘      └─────────────┘
                            │
                            │
                     ┌──────▼──────┐
                     │   Solana    │
                     │ Blockchain  │
                     └─────────────┘
```

## License

MIT

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## Contact

For questions, support, or collaboration opportunities:

- **Telegram**: [@blategold](https://t.me/blategold)

---

<div align="center">

**Built with ❤️ on Solana**

[Documentation](./PROJECT_STRUCTURE.md) • [Backend API](./backend/README.md) • [Smart Contracts](./contracts/solana/README.md)

</div>

