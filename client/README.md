<p align="center">
  <a href="https://github.com/ankitrekha01/RCE">
  </a>

  <h3 align="center">Remote Code Executor</h3>
</p>

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

This is the FrontEnd code of a Remote Code Executor. This is a project assigned by the Coding forum of my college and is similar to the Online IDEs of websites like CodeChef and Leetcode.

Salient Features:

- Code Sanitisation
- An individual Docker Container is created for every code posted on the API, so no code interferes with any other code
- All Async code so that the server can handle multiple requests without error
- Socket has been implemented along with rooms for seperate users so that the server can handle multiple users in multiple rooms
- Keeping it simple, there is not need for signup or login, you can jump in and start coding
- Timeouts and max memory have been implemented so that no code takes up too much of the server's time
- Implemented SwaggerUI as an API Sandbox so anyone can explore endpoints and familiarize themselves with the server
- Timeout to prevent the user from spamming the run code button and triggering a DoS attack
- Adequate toasts have been implemented so that anyone in the room is alerted if anyone joins or leaves
- No duplicate usernames are allowed
- In case a user loses internet, he will be taken back to the Join Page, and will be prompted to login again
- Completely responsive so people on mobile can use this RCE as well.

### Built With

<a href="https://expressjs.com" target="_blank"> <img src="https://www.vectorlogo.zone/logos/expressjs/expressjs-ar21.svg" alt="express" height="40"/> </a><a href="https://reactjs.org/" target="_blank"> <img src="https://upload.wikimedia.org/wikipedia/commons/a/a7/React-icon.svg" alt="react" width="60" height="40"/> </a><a href="https://nodejs.org" target="_blank"> <img src="https://img.icons8.com/color/48/000000/nodejs.png"/> </a>
<a href="https://www.docker.com/" target="_blank"> <img src="https://www.docker.com/sites/default/files/d8/styles/role_icon/public/2019-07/Moby-logo.png?itok=sYH_JEaJ" alt="docker" width="58" height="50"/> </a> 

<!-- GETTING STARTED -->

## Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

- npm
  ```sh
  npm install npm@latest -g
  ```
- yarn
  ```sh
  npm install -g yarn
  ```

### Installation
1. Clone the repo
   ```sh
   git clone https://github.com/ankitrekha01/RCE
   ```
2. Install NPM packages
   ```sh
   npm install
   ```
3. Or using yarn
   ```sh
   yarn install
   ```
<!-- USAGE EXAMPLES -->

## Usage

- To run the React App with npm
  ```sh
  npm start
  ```
- To run the React App with yarn
  ```sh
  yarn start
  ```
- It is important to note that you will have to setup environment variables to the appropriate endpoints, should you deploy this locally or somewhere else



## License

Distributed under the MIT License. See `LICENSE` for more information.

<!-- CONTACT -->


## Screenshots
<img src="https://i.imgur.com/FOKwshQ.png"></img>
<img src="https://i.imgur.com/lb6Mcjx.png"></img>
<img src="https://i.imgur.com/npnqlZb.png"></img>
<img src="https://i.imgur.com/QxxhIju.png"></img>
<img src="https://i.imgur.com/OtICDoU.png"></img>
