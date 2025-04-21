# DecaStream

🚀 A fully decentralized, censorship-resistant, open live streaming network.

## 🎯 Vision

DecaStream aims to be the Web3-native infrastructure for livestreaming. Unlike centralized platforms, it allows anyone to broadcast without permission, censorship, or cost limitations—by contributing to the network.

### Core Principles:
- **Free to stream**: Anyone can start pushing a livestream without paying.
- **Incentive to contribute**: Users who provide transcoding or storage nodes earn tokens.
- **No central server**: All content is pushed, encoded, and distributed through community nodes.
- **Token-governed economy**: Streamers either contribute or pay small tokens to use network resources.

## 🧱 Architecture Overview

### Modules:

- **Ingest Gateway**: Accept RTMP/SRT/WHIP live inputs from OBS or any streaming software.
- **Transcoding Node**: Docker container that takes live stream, encodes to HLS/DASH at multiple bitrates.
- **Distributed Storage**: IPFS or other decentralized networks to cache segments for viewers.
- **Viewer Player**: Web app or desktop player that supports HLS and IPFS protocols.
- **Blockchain Layer**: Ethereum-compatible smart contracts for rewarding contributors.

## 📦 Repository Structure (Planned)

```
decastream/
├── README.md
├── docs/
│   ├── vision.md              # Extended vision
│   ├── architecture.md        # Architecture diagrams
│   └── roadmap.md             # Milestones and task breakdown
├── node/
│   └── transcode-node/        # FFmpeg-based worker
├── gateway/
│   └── ingest/                # RTMP/SRT handling and relay
├── blockchain/
│   └── contracts/             # Token & reward contract (Solidity)
└── frontend/
    └── player/                # Decentralized viewer (HLS+IPFS)
```

## 🛠 Getting Started

1. Clone the repo: `git clone https://github.com/decastream/decastream`
2. Run your first node: `cd node/transcode-node && docker compose up`
3. Push RTMP stream to the gateway.
4. Watch from the decentralized web player.

## 👥 Join the Community

We are recruiting contributors who are interested in:
- WebRTC, RTMP, and streaming protocols
- P2P file systems (IPFS, Arweave)
- Smart contracts and tokenomics
- Fullstack streaming applications

📣 Join our Discord to discuss ideas, propose improvements, and help us build the future of unstoppable streaming.

https://discord.gg/gS7DCj68
