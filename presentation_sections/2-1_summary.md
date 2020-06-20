# Overview
## Event Sourcing / C.Q.R.S / D.D.D.



## D.D.D. - Domain Driven Design

Domain Driven Design is the idea that a software system should match the real-world domain that it is being built for.

- Context
- Domain
- Model
- Ubiquitous Language

Note:

Domain driven design is the idea that a software system should match the real-world domain it is being build for.
Or at least as closly as possible.

To acheive this, DDD, has 3 major concepts to consider.

Context is not a software idea, but rather the context in which word and statements live.

The Domain refers to a sphere of knowledge and activity. Our domain is Amazon.

The model used is an abstraction of real-world aspects of the domain that are used to solve problems in the domain
> Ex. We have the idea of a listing in Amazon, that is part of the model



<img style="width: 100%; height: 100%; top: 50%;" alt="ddd" src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse3.mm.bing.net%2Fth%3Fid%3DOIP.lIXrwMFYpjuV7eSrPJ6nbAHaFX%26pid%3DApi&f=1" />



## C.Q.R.S. - Command Query Responsibility Separation

C.Q.R.S. is the concept that the command that a user sends to perform an action should be separated from the events that change the system.

- Keeping an audit log
- Extendable and flexable systems
- Scalability

Note:

C.Q.R.S. is the concept that the command that a user sends to perform an action should be separated from the events that change the system.

It is a simple but powerful concept, and we will come to see how keeping command and queries separate can help us build bulletproof systems.

We will explore using command as an audit log, Making systems extendable and flexable and using CQRS to improve scalability.



<img style="width: 100%; height: 100%; top: 50%;" alt="ddd" src="https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fi.imgur.com%2Fa5R8oEk.png&f=1&nofb=1" />



## Event Sourcing

Instead of keeping a record of only the current state of the data within a system, Event Sourcing keeps a record of the full series of actions taken on thats data

- Append-only systems
- Events are understandable for Domain Experts and Developers
- Event Stores
- More...

Note:

Instead of keeping a record of only the current state of the data within a system, Event Sourcing keeps a record of the full series of actions taken on thats data

We will explore the benefits of an append-only system.

We will explore where events come from, hint: they come from the domain

And then we will look at the idea of an eventstore. How and why it is used.



<img style="width: 100%; height: 100%; top: 50%;" alt="ddd" src="https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fprolic.github.io%2Fcqrs-event-sourcing-talk%2Fassets%2Fimg%2Fcommand-event-event-store.png&f=1&nofb=1" />
