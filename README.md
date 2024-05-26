# robinclone

## About

I'm learning about creating scalable applications and system design, and wanted to write an application from scratch.

## Functionality

- Users create accounts for their portfolios
- Users can view current data for a specific stock symbol
- Users can buy/sell holdings of said symbol
- Users can check their portfolio to see how their stocks are doing, using real-time data
- Users can deposit money from a bank (notional for this project)

## Goals

_Note_: Goals are broken down in their respective branches.

For example, Goal 1 is in branch `1-base-app`.

1. Create the base web-app
    - Python Flask (server-side)
    - HTML/CSS/JS (client-side)
    - Local sqlite database for storing user info
2. Separate data tier from web tier
    - Utilize a separate NoSQL or Postgres server to handle data operations
3. Scale web tier
    - Utilize Kubernetes to orchestrate a load balancer and replica pods for web tier
4. Scale data tier
    - Employ sharding on data tier for higher fault tolerance and faster operations
    - Utilize a cache layer for operations to data tier
5. Monitoring, metrics, and analytics
    - Set up monitoring for the system to track performance and issues
6. Message queue
    - Employ a message queue to handle buy/sell requests asynchronously
