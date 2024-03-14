# FeedAndFandom

## Overview

A full-stack web platform for a creator to share recipes, videos, and articles, and engage with fans. Built with React, Node.js, Express, and PostgreSQL, it supports content management and interactive fan suggestions, fostering a vibrant community around the creator's culinary and creative journey.

## Features

- **Recipe Management**: Allows the creator to add, edit, and delete recipes with details like ingredients, instructions, and images.
- **Video and Article Sharing**: Enables posting and managing favorite videos and articles with options for descriptions or comments.
- **Fan Interaction**: Facilitates fan submissions of content suggestions, allowing the creator to engage with their community.

## Technologies

- **Frontend**: Next.js
- **Backend**: Next.js
- **Database**: PostgreSQL
- **Others**: Knex.js for database migrations, Netfily and Heroku for deployment

## Getting Started

### Prerequisites

- Node.js
- PostgreSQL

### Installation

1. Clone the repository:
   ``` cmd
   git clone https://github.com/ivancuadra93/FeedAndFandom.git
   ```
2. Run docker to start up both the server and database containers:
    ``` cmd
    docker compose up --build
    ```
    You can run `docker ps` to view the containers that are running.
   
4. Set up the database by configuring PostgreSQL and running the necessary migrations and seeds:
   ``` cmd
   docker exec <container-id> npx prisma migrate dev
   docker exec <container-id> npx prisma db seed
   ```

### Querying the Database

1. You view the database schemas and tables, as well as run queries by using psql:
   ``` cmd
   docker exec -it <container-id>  psql -d <db-name>
   ```
   
2. You can also use pgAdmin with host name host.docker.internal and port 5432
  
### Running the Application

WIP

## Project Structure

WIP
