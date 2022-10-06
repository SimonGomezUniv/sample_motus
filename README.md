# Sample motus App

## Description 

Sample motus app
to start with microservice course

 ## Usage 
 
 use with standard node command
 
 ```
 npm install
 node index.js
 ```

go to http://localhost:4000



## how it work ?

On loading, the page get the current word and all is done localy.

```mermaid

sequenceDiagram
    Client->>+Server: /
    Server->>+Client: index
    Client->>Server:/word
    Server->>Client:Word_TO_GUESS
    Note left of Client: Guessing
    Client->>Client: Guessing and storing info to localstorage
    Client->>Server:score.html
    Server->>Client: score.html
    Client->>Client : load score from local storage
    
 ```
