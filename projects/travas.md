---
layout: page
title: Travas Platform
permalink: /projects/travas/
---

![Travas](/assets/images/travas_001.png)

## Overview
Cryptocurrency trading strategy design and live deployment platform.

## Technologies Used
- **Java Spring Boot**: API and websocket servers
- **JavaScript React**: Frontend application
- **Arch Linux**: dedicated servers for staging and production environments
- **MySQL**: database used for application data on dedicated server

## Description
The Travas Platform was the core product of Travas, Inc a company I founded alongside two others.  The project's core use case was to provide an all-in-one solution for creating and deploying automated trading strategies for hundreds of cryptocurrency markets.  The platform integrated with several APIs and websockets to enable live market price monitoring and trading bot automation.  

Travas leveraged a large suite of technologies ranging from public and private APIs to dedicated websocket servers used for running automated trading bots and sending events to clients.  The platform was deployed on a series of dedicated servers and sat behind a Cloudflare gateway which provided round-robin load balancing and DDoS protection.

The backend primarily utilized Java Spring Boot to provide APIs to the frontend as well as websockets available for automated trading systems.  The backend also implemented and tested hundreds of trading indicators which could be used inside complex strategies and both back-tested and forward-tested.

## Key Features
- Strategy design: Mix and match indicators and custom criteria for an automated trading strategy
- Strategy deployment: Deploy strategy to a bot which runs 24/7 over a selected cryptocurrency market
- Backtesting: Run a strategy over a historical set of data to compare performance to Bitcoin buy and hold
- Account management: Update account information, add and remove API keys

## What I Learned
I probably learned more working on Travas than any other project I worked on in my life.  This was the first time I built and deployed a distributed application for real-time usage.  I covered many different areas, listed below:

- Automated deployments to dedicated servers
- Websocket technology using Spring Boot
- Cloudflare for load balancing and DDoS protection
- IP lists for whitelisting IPs for backend servers using static IPs
- Setting up DNS entries for domain name mapping for production and staging environments
- Preparing and presenting to potential investors
- Securing sensitive database data using encryption and rolling secret keys
- Working with beta testers to fix and enhance existing features
- First time using JavaScript React
- API and frontend data caching
- Testing and deployment of live real-time systems
- Updating live running systems

## Links
- [GitHub: Backend](https://github.com/dtand/travas-backend)
- [GitHub: Frontend](https://github.com/dtand/travas-frontend)

## Attachments
- [Travas Slide Decks](/assets/travas_slide_decks.pptx)

[← Back to Projects](/projects/)
