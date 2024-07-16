# Deploying My Node.js Application with MongoDB and Mongo-express on EC2 on AWS server

## Overview

This project is a **Node.js** application that uses **MongoDB** to store user profiles. The application serves static files, including an HTML file and an image, and provides endpoints for updating and fetching user profiles. It can run locally, in a Docker container, or as part of a Docker Compose setup.

## Table of Contents

- **Overview**
- **Prerequisites**
- **Installation**
  - *Local Setup*
  - *Docker Setup*
- **Usage**
- **Endpoints**
- **Docker**
  - *Running with Docker*
  - *Running with Docker Compose*
- **Contributing**
- **License**

## Prerequisites

To run this application locally or in a Docker container, you need the following:

- Node.js
- MongoDB
- Docker (optional, for running with Docker)
- Docker Compose (optional, for running with Docker Compose)

## Installation

### Local Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
2. Install dependencies:
   ```bash
   npm install

### Docker Setup

Docker Setup
Build the Docker image (if not already built): 
    ```bash
    
    docker build -t my-node-app .

## Run the Docker container:

    ```bash
    
        docker run -p 3000:3000 -e MONGO_URL=mongodb://admin:password@host.docker.internal:27017 my-node-app

## Usage
Ensure MongoDB is running and accessible.

Set the environment variable MONGO_URL for MongoDB connection (if different from the default).

## Start the application:

 ```bash
     npm start
    Open your browser and navigate to http://localhost:3000.

## Docker
Running with Docker
Build the Docker image (if not already built):

    ```bash
docker build -t my-node-app .

## Run the Docker container:

    ```bash
docker run -p 3000:3000 -e MONGO_URL=mongodb://admin:password@host.docker.internal:27017 my-node-app

## Running with Docker Compose
Ensure Docker Compose is installed.
Create a docker-compose.yml file in the root directory:
