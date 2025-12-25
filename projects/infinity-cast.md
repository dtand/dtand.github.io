---
layout: page
title: Infinity Cast
permalink: /projects/infinity-cast/
---

![Infinity Cast](/assets/images/infinity-cast-001.png)

## Overview
Infinity Cast is a web application which hosts thousands of short-form AI-generated podcasts. Infinity Cast is a partially complete MVP passion and budget project.

## Technologies Used
- **JavaScript React with Typescript**: frontend implementation
- **NodeJS**: API implementation
- **Google Gemini**: podcast topic and script generation
- **Google Gemini TTS**: podcast audio generation
- **N8N**: backend workers, jobs and admin APIs
- **Postgres**: main data store for application
- **Amazon S3**: podcast audio and cover art storage
- **Simple Diffuse**: podcast cover art generation

## Description
Infinity Cast aims to be a platform for both producing and consuming short-form podcasts. Short-form in the context of podcasts are podcasts ranging between 4 and 5 minutes in length.

Infinity Cast leverages the Google Cloud suite along with Gemini APIs to generate podcast topics, scripts and audio. The platform hopes to provide a unique experience for digesting content, primarily through unique playlist topics and endless topic generation. The eventual goal is to allow users to generate and share playlists with other users.

## Key Features
- Authentication and guest flows using JWT and OAuth
- Creation of playlists
- Podcast search with input text and filters
- Generate podcast from description (currently disabled)

## What I Learned
This was a fascinating project, and the first project I have heavily integrated with existing AI tools. I learned how to work effectively with generated code using Claude Sonnet integrated into my IDE to quickly get a full application up and running within weeks. I also explored other concepts and technologies that I had not used before including: Google Gemini APIs, OAuth integration, N8N workflows and Simple Diffuse APIs for image generation.

## Links
- [GitHub Repository](#)
- [Live Application](https://infinity-cast-app-a53d4055355c.herokuapp.com/)

[← Back to Projects](/projects/)
