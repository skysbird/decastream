# Architecture Overview

## 🧱 Core Modules
[ OBS/RTMP ] --> [ Gateway ] | v [ Transcoder Node ] | v [ IPFS/Storage Layer ] | v [ Smart Contracts ] | v [ Player Frontend ]

## 🔧 Components

- **Ingest Gateway**
  - Accepts RTMP/WHIP/SRT
  - Validates input, splits into segments
- **Transcoder Node**
  - FFmpeg in Docker
  - Generates HLS/DASH
  - Optional: watermarking / signature
- **Storage**
  - IPFS, Arweave or custom P2P storage
- **Smart Contracts**
  - Rewards for node operators
  - Token staking or bandwidth tracking
- **Frontend Player**
  - React/Vite or Web-based player
  - Loads from decentralized sources

