<h3 align="center">Remote Code Executor</h3>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#screenshots">Screenshots</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

## About The Project

This is a Remote Code Executor, virtual platform where you can write, edit, and run your code directly within a web browser. It is similar to the Online IDEs of websites like CodeChef and Leetcode.

Salient Features:

- An individual Docker Container is created for every code posted on the API, so no code interferes with any other code
- All Async code so that the server can handle multiple requests without error
- Socket has been implemented along with rooms for seperate users so that the server can handle multiple users in multiple rooms
- Keeping it simple, there is not need for signup or login, you can jump in and start coding
- Timeouts and max memory have been implemented so that no code takes up too much of the server's time
- Timeout to prevent the user from spamming the run code button and triggering a DoS attack
- Stay informed with real-time notifications when users join or leave the meeting room, keeping you updated on participant activity.
- In the event of an internet interruption, the user will be gracefully redirected back to the Join Page, where they will be prompted to log in again
- To maintain a unique and distinct user environment, duplicate usernames are not permitted. 

### Built With

<a href="https://expressjs.com" target="_blank"> <img src="https://www.vectorlogo.zone/logos/expressjs/expressjs-ar21.svg" alt="express" height="40"/> </a><a href="https://reactjs.org/" target="_blank"> <img src="https://upload.wikimedia.org/wikipedia/commons/a/a7/React-icon.svg" alt="react" width="60" height="40"/> </a><a href="https://nodejs.org" target="_blank"> <img src="https://img.icons8.com/color/48/000000/nodejs.png"/> </a>
<a href="https://www.docker.com/" target="_blank"> <img src="https://www.docker.com/wp-content/uploads/2022/03/vertical-logo-monochromatic.png" alt="docker" width="40" height="40"/> </a> 
<a href="https://socket.io/" target="_blank"> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/96/Socket-io.svg/1200px-Socket-io.svg.png" alt="SocketIO" width="40" height="40" /></a>

<!-- GETTING STARTED -->

## Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

- npm
  ```sh
  npm install npm@latest -g
  ```
- docker
  ```sh
  curl -fsSL https://get.docker.com -o get-docker.sh
  ```
  ```sh
  sudo sh get-docker.sh
  ```

### Installation
#### If you are on a Linux Machine
1. Clone the repo
   ```sh
   git clone https://github.com/ankitrekha01/RCE
   ```
2. Install NPM packages
   ```sh
   npm install
   ```
3. To build the docker images
   ```sh 
   cd Dockerfiles 
   ```
   ```sh 
   docker build -t cpp:v1 -f DockerCPP . 
   ```
   ```sh 
   docker build -t python:v1 -f DockerPython . 
   ```
   ```sh 
   docker build -t java:v1 -f DockerJava . 
   ```
   ```sh 
   docker build -t go:v1 -f DockerGo . 
   ```
   ```sh
   docker build -t c:v1 -f DockerC .
   ```
#### If you are on any other Machine
1. Clone the repo
   ```sh
   git clone https://github.com/ankitrekha01/RCE
   ```
2. Install NPM packages
   ```sh
   npm install
   ```
3. Build the Server's Dockerfile
   ```sh
   docker build -t rceserver:v1 .
   ```
4. Run the Docker Image
   ```sh
   docker run --privileged=true -v /var/run/docker.sock:/var/run/docker.sock -d -p 3000:3000 rceserver:v1  
   ```
5. Create a shell to the created Docker Container
   ```sh
   docker ps
   ```
   ```sh
   docker exec -it <container_id> /bin/bash
   ```
6. Build the Images inside the Container
   ```sh 
   cd Dockerfiles 
   ```
   ```sh 
   docker build -t cpp:v1 -f DockerCPP . 
   ```
   ```sh 
   docker build -t python:v1 -f DockerPython . 
   ```
   ```sh 
   docker build -t java:v1 -f DockerJava . 
   ```
   ```sh 
   docker build -t go:v1 -f DockerGo . 
   ```
   ```sh
   docker build -t c:v1 -f DockerC .
   ```
<!-- USAGE EXAMPLES -->

## Usage

1.  To run the App and server

    - To run the React App(FrontEnd)
    ```sh
    npm start
    ```
    - To run the server(BackEnd)

      - In dev mode
      ```sh
      npm run dev
      ```
      - In production mode
      ```sh
      npm start
      ```
2.  Note that dev mode uses nodemon so that the server can be changed and restarted easily

## Screenshots
<img src="https://i.imgur.com/QxxhIju.png"></img>
<img src="https://i.imgur.com/OtICDoU.png"></img>
