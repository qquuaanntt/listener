# listener

## Overview
`listener` is a Rust-based application that connects to an Ethereum WebSocket provider and listens for new pending transactions. This guide will help you get set up from scratch.

## Prerequisites
Before you begin, ensure that you have the following:
- A computer running macOS, Linux, or Windows
- An internet connection
- Access to a command line interface

## Step 1: Install Rust
If you don't have Rust installed, you can follow the instructions on the [official Rust website](https://www.rust-lang.org/tools/install).

## Step 2: Clone `listener`

```bash
git clone https://github.com/qquuaanntt/listener.git
cd listener
```

## Step 3: Set Up Environment Variables
`listener` requires a `.env` file to store configuration values. Create a `.env` file in the root of the `listener` directory:

```bash
touch .env
```

Add the following line:

```env
WS_URL="ws://your-websocket-url:8546"
```

Replace `"ws://your-websocket-url:8546"` with the URL of your Ethereum WebSocket provider.

## Step 4: Build the project

```bash
cargo build
```

## Step 5: Run `listener`

```bash
cargo run
```

If everything is set up correctly, you should see logs in your terminal indicating that you are connected to the Ethereum node and processing transactions.
