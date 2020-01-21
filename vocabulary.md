# Under Construction
## What is this?
A central file with the definitions of all terms used inside the company, from product specific terms to technical ones.

## Why?
Because we need to speak the same language and have that common understanding of a term when it is used in a discussion or a presentation.

## Glossary

* [Product](#product)
* [Process](#process)
* [AI](#ai)
* [Dev](#dev)
* [Playground](#playground)

## Product
Specific terms that we use at all levels, from business to product and tech.

### Code Generators
A collection of open source libraries used to generate modern frontend application code, based on our UI representation (UIDL). The code for the library is available on github under a monorepo [here](https://github.com/teleporthq/teleport-code-generators). The docs can be consulted at https://docs.teleporthq.io/.

### Design System

### Open Source

### Playground

### UIDL
UIDL or openUIDL is a human-readable JSON document, a format supported natively by many programming languages, and easy to manipulate. There are two types of UIDLs: componentUIDL and projectUIDL.

Component UIDL example:
```json
{
  "name": "Simple Component",
  "propDefinitions": {
    "heading": {
      "type": "string",
      "defaultValue": "Hello"
    }
  },
  "node": {
    "type": "element",
    "content": {
      "elementType": "container",
      "children": [
        {
          "type": "element",
          "content": {
            "elementType": "text",
            "children": [
              {
                "type": "dynamic",
                "content": {
                  "referenceType": "prop",
                  "id": "heading"
                }
              },
              {
                "type": "static",
                "content": "World!"
              }
            ]
          }
        }
      ]
    }
  }
}
```

Although at the beginning the role of the UIDL seemed to be limited to describing the UI elements and their relationship, we are now confident that we can use it also to describe user interactions, flows, events, and more complicated UI patterns based on component architectures and dynamic data driven applications.

You can further play with component UIDLs in the [online REPL](https://repl.teleporthq.io/).

### VisionAPI

### Vision2Teleport

## Process

Terms related to our way of working and collaboration tools.

### Board

### Code Review

### Daily

### Retro

## AI

Technical terms related to AI and ML. For general purpose AI terms, consult [this link](https://developers.google.com/machine-learning/glossary).

## Dev

Technical terms related to JavaScript and Software Development/Architecture

### Domain Driven Design

### Event Sourcing

### Monorepo

## Playground

Terms which are specific for the **playground**.

### Dashboard

### Inspector

### Stage
