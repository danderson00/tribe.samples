# Samples for the tribe Platform

## Installation

    git clone https://github.com/danderson00/tribe.samples.git
    cd tribe.samples
    npm install

## Running

Change to the directory containing the desired sample and run

    node --debug ./server.js

Open a browser to `http://localhost:1678/`. Note that these samples require
node 4.0.0 or above and a browser that supports arrow functions (Chrome).

By default, the server uses a SQLite in memory database. Use `ctrl-]` in the
browser to reset the client side message cache after restarting the server.

## Samples

### chat

#### widget

A minimalistic sample showing basic publishing and subscribing. Try opening
multiple windows.

#### rooms

The same chat widget used in isolated "rooms". Introduces the concept of scope.

#### actor

Encapsulates the concept of a chat room in an actor, exposing a model through
the actor's public interface. We don't actually want to do this - it is an
anti-pattern, old-school OO thinking; modelling a "snapshot" of reality.

#### application

A more comprehensive chat application, with user names and some styling.

### score

A simple scoring application for point based games, intended to be used on
mobile devices.

A few concepts are introduced here:

- Expressions: Declaratively bind UI elements and actor message handlers
  using the power of Rx expressions.
- Flows: Syntactic sugar over actors to control navigation from events in
  simple, decoupled modules. Think FSM.
- Vocabulary: Custom expressions that can be used throughout the application
  to construct a more natural language.

## Feedback? Broken?

- https://github.com/danderson00/tribe.samples/issues
- https://twitter.com/danderson00
