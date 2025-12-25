---
layout: page
title: Essencion Card Game
permalink: /projects/essencion/
---

![Essencion](/assets/images/essencion-gameplay.png)

## Overview
Essencion is a peer-to-peer collectible card game (CCG) that runs on the web using WebSocket technology.

## Technologies Used
- **JavaScript React**: frontend
- **Java Spring Boot**: websocket technology for peer-to-peer gameplay
- **Redis**: in-memory caching of game state for player sessions
- **Python Flask**: public APIs for cards and deck-building
- **NodeJS**: authentication service using JWTs
- **AWS S3 Buckets**: storage for card images
- **Solana**: SPL token generation
- **Postgres**: primary data store
- **Golang**: matchmaking API service

## Architecture

![Essencion Architecture](/assets/images/essencion-architecture.png)

## Description
Essencion is a digital CCG, akin to Hearthstone, but it differs significantly in its game mechanics. The game is designed specifically to run in the browser, allowing it to be platform-agnostic and highly available. This is achieved through the use of WebSocket technology and the pub/sub model. Additionally, many microservices are used to coordinate and provide the main functionality required for the application.

## Key Features
- Card viewer and deck builder UIs
- Player matchmaking queue
- Peer-to-peer gameplay
- Interactive gameplay UI (in-browser)
- Solana SPL token rewards per game
- Public API for the card viewer
- User-based API for deck-building

## Game Rules
1. Each player has a deck of 25 cards
2. Players draw 5 cards each to start
3. Player going first is chosen at random
4. Each player can have up to 9 mana, starting at 2 max and gaining 1 max each turn
5. During each player's turn:
    - Player starts with max mana
    - Summon a minion
    - Play a support card
    - Pass turn
6. Minion cards - may have abilities and can attack opposing minions

   ![Minion Card Example](/assets/images/minion.png)

7. Support cards - immediately perform specified ability

   ![Support Card Example](/assets/images/support.png)

8. Essence is assigned to each minion; when the minion is defeated, the opponent collects essence

9. The first player to get to 50 essence "ascends" and wins the game

## What I Learned
This project covered many different areas. This was my first time working with the Solana blockchain. I learned about minting NFTs on-chain, as well as minting tokens for use on the platform. I also used Golang for the matchmaking engine, which was my first experience with the language.

Other notable technologies I used for the first time while building this application include Amazon S3, JSON Web Tokens, and Redis (used for caching live game state in memory).

## Links
- [Github: Game Server](https://github.com/dtand/essencion-game-server)
- [Github: Frontend](https://github.com/dtand/essencion_card_game_frontend)
- [Github: Matchmaking Service](https://github.com/dtand/essencion_matchmaking)
- [Github: Card Game API](https://github.com/dtand/essencion-card-game-api)
- [Github: Token Server](https://github.com/dtand/essension-token-server)

[← Back to Projects](/projects/)
