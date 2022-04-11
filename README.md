# Peer To Peer Exchange

This project provides a website for everyone to buy and sell Cryptocurrency in a peer to peer way.
The Users won't be tracked. The only information they provide to the website is their telegram username. 

When creating an entry on the website the information will be sent to the backend and saved in a MySQL database. 

## Database tables

### ```buyers```

| idbuyers | pair | amount | location | contact | password |
| --- | --- | --- |--- | --- | --- |
| int | string | float | string | string | string |

### ```sellers```

| idsellers | pair | amount | location | contact | password |
| --- | --- | --- |--- | --- | --- |
| int | string | float | string | string | string |

## client-with-snel

Peer 2 Peer Exchange frontend working with snel <https://github.com/crewdevio/Snel>

## Run server

To run the webpage you have to start the snel frontend and the deno backend. 
The deno backend should be connected to a MySQL database.

#### Run Snel Frontend

`trex run start`

#### Run deno Backend

`deno run --allow-net --allow-read .\server.ts 443`

## Where to reach the server

https://dvdope.github.io/

## Future improvements

* Complete Repo
* Put server.ts into docker container
* Show password to delete entry after creation
* Delete entries after n days
