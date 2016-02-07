# Samples for the tribe Platform

## Installation

    git clone https://github.com/danderson00/tribe.samples.git
    npm i

For integrated server side debugging

    npm i node-inspector

## Running

Change to the directory containing the desired sample

    node --debug ./server.js

Open a browser to `http://localhost:1678/`. Note that these samples require
node 4.0.0 or above and a browser that supports arrow functions (Chrome).

By default, the server uses a SQLite in memory database. Use `ctrl-]` in the
browser to reset the client side message cache after restarting the server.