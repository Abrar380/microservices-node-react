## **Section 15: Connecting to NATS in a Node JS World**

## Table of Contents
- [**Section 15: Connecting to NATS in a Node JS World**](#section-15-connecting-to-nats-in-a-node-js-world)
- [Table of Contents](#table-of-contents)
  - [Reusable NATS Listeners](#reusable-nats-listeners)
  - [The Listener Abstract Class](#the-listener-abstract-class)
  - [Extending the Listener](#extending-the-listener)
  - [Quick Refactor](#quick-refactor)
  - [Leveraging TypeScript for Listener Validation](#leveraging-typescript-for-listener-validation)
  - [Subjects Enum](#subjects-enum)
  - [Custom Event Interface](#custom-event-interface)
  - [Enforcing Listener Subjects](#enforcing-listener-subjects)
  - [Quick Note: 'readonly' in Typescript](#quick-note-readonly-in-typescript)
  - [Enforcing Data Types](#enforcing-data-types)
  - [Where Does this Get Used?](#where-does-this-get-used)
  - [Custom Publisher](#custom-publisher)
  - [Using the Custom Publisher](#using-the-custom-publisher)
  - [Awaiting Event Publication](#awaiting-event-publication)
  - [Common Event Definitions Summary](#common-event-definitions-summary)
  - [Updating the Common Module](#updating-the-common-module)
  - [Restarting NATS](#restarting-nats)

### Reusable NATS Listeners

- Wow, this is a lot of boilerplate to publish/receive a message!
- Let's try to refactor this to make it much easier to publish/receive
- We'll write out an initial implementation in this test project, then move it to our common module

![](section-15/class-listener-1.jpg)
![](section-15/class-listener-2.jpg)

**[⬆ back to top](#table-of-contents)**

### The Listener Abstract Class
**[⬆ back to top](#table-of-contents)**

### Extending the Listener
**[⬆ back to top](#table-of-contents)**

### Quick Refactor
**[⬆ back to top](#table-of-contents)**

### Leveraging TypeScript for Listener Validation
**[⬆ back to top](#table-of-contents)**

### Subjects Enum
**[⬆ back to top](#table-of-contents)**

### Custom Event Interface
**[⬆ back to top](#table-of-contents)**

### Enforcing Listener Subjects
**[⬆ back to top](#table-of-contents)**

### Quick Note: 'readonly' in Typescript
**[⬆ back to top](#table-of-contents)**

### Enforcing Data Types
**[⬆ back to top](#table-of-contents)**

### Where Does this Get Used?
**[⬆ back to top](#table-of-contents)**

### Custom Publisher
**[⬆ back to top](#table-of-contents)**

### Using the Custom Publisher
**[⬆ back to top](#table-of-contents)**

### Awaiting Event Publication
**[⬆ back to top](#table-of-contents)**

### Common Event Definitions Summary
**[⬆ back to top](#table-of-contents)**

### Updating the Common Module
**[⬆ back to top](#table-of-contents)**

### Restarting NATS
**[⬆ back to top](#table-of-contents)**