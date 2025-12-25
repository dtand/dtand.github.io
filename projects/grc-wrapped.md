---

layout: page
title: GRC Wrapped
permalink: /projects/grc-wrapped/
---

![GRC Wrapped](/assets/images/grc-wrapped.png)

## Overview
A year-in-review analytics dashboard for GRC data.

## Technologies Used
- **JavaScript React w/ TypeScript**: Frontend application
- **Golang**: backend API
- **Python**: utility scripts
- **Postgres**: database persistence layer

## Description
GRC Wrapped is a full-stack application that aims to compile and normalize historical running club data and present it in a meaningful way. The application defines and implements a large API spec for various functionality and also provides capabilities for parsing and injecting new performance data for athletes. The backend integrates with the Anthropic API and uses Claude to help parse out key data from unstructured email summaries.

## Key Features
- Dashboard
- Athlete Performances
- REST API Layer
- Claude API
- Data Injection

## What I Learned
Parsing unstructured emails for data can be challenging. I was leveraging the Claude API to help pull out specific details for clubmates' race performances and learned the importance of very specific context. In order to get the best result, I had to provide the entire club roster along with nickname mappings and very specific details and requirements for the parsing. I learned that Claude is able to get about 80% there, then some manual work needed to be done using the specific knowledge I have about running and my clubmates to correct some of the race distances. There were some other interesting challenges such as handling ambiguity with conflicting athlete names, in these cases the race performance was flagged and reviewed manually.

## Links
- [GitHub Repository](https://github.com/dtand/grc-wrapped)
- [Live App](https://grc-app-frontend-8839ec2851e0.herokuapp.com/)

[← Back to Projects](/projects/)
