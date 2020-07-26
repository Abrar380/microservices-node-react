## **Section 22: Back to the Client**

## Table of Contents
- [**Section 22: Back to the Client**](#section-22-back-to-the-client)
- [Table of Contents](#table-of-contents)
  - [A Few More Pages](#a-few-more-pages)
  - [Reminder on Data Fetching with Next](#reminder-on-data-fetching-with-next)
  - [Two Quick Fixes](#two-quick-fixes)
  - [Scaffolding a Form](#scaffolding-a-form)
  - [Sanitizing Price Input](#sanitizing-price-input)
  - [Ticket Creation](#ticket-creation)
  - [Listing All Tickets](#listing-all-tickets)
  - [Linking to Wildcard Routes](#linking-to-wildcard-routes)
  - [Creating an Order](#creating-an-order)
  - [Programmatic Navigation to Wildcard Routes](#programmatic-navigation-to-wildcard-routes)
  - [The Expiration Timer](#the-expiration-timer)
  - [Displaying the Expiration](#displaying-the-expiration)
  - [Showing a Stripe Payment Form](#showing-a-stripe-payment-form)
  - [Configuring Stripe](#configuring-stripe)
  - [Test Credit Card Numbers](#test-credit-card-numbers)
  - [Paying for an Order](#paying-for-an-order)
  - [Filtering Reserved Tickets](#filtering-reserved-tickets)
  - [Header Links](#header-links)
  - [Rendering a List of Orders](#rendering-a-list-of-orders)

### A Few More Pages

![](section-22/page-1.jpg)
![](section-22/page-2.jpg)
![](section-22/page-3.jpg)
![](section-22/routes.jpg)

**[⬆ back to top](#table-of-contents)**

### Reminder on Data Fetching with Next

![](section-22/next-1.jpg)
![](section-22/next-2.jpg)

**[⬆ back to top](#table-of-contents)**

### Two Quick Fixes

- Type 'thisisunsafe' in Chrome to bypass security warning
- Fetch getCurrentUser in _app.js and index.js

```javascript
const AppComponent = ({ Component, pageProps, currentUser }) => {
  // Fix #1: pass currentUser directly into Component
  return (
    <div>
      <Header currentUser={currentUser} />
      <Component currentUser={currentUser} {...pageProps}  />
    </div>
  );
};

AppComponent.getInitialProps = async appContext => {
  const client = buildClient(appContext.ctx);
  const { data } = await client.get('/api/users/currentuser');

  let pageProps = {};
  if(appContext.Component.getInitialProps) {
    // Fix #2
    pageProps = await appContext.Component.getInitialProps(appContext.ctx, client, data.currentUser);
  }

  return {
    pageProps,
    ...data
  };
};

export default AppComponent;
```


**[⬆ back to top](#table-of-contents)**

### Scaffolding a Form

```javascript
const NewTicket = () => {
  return (
    <div>
      <h1>Create a Ticket</h1>
      <form>
        <div className="form-group">
          <label>Title</label>
          <input className="form-control" />
        </div>
        <div className="form-group">
          <label>Price</label>
          <input className="form-control" />
        </div>
        <button className="btn btn-primary">Submit</button>
      </form>
    </div>
  );
};

export default NewTicket;
```

**[⬆ back to top](#table-of-contents)**

### Sanitizing Price Input
**[⬆ back to top](#table-of-contents)**

### Ticket Creation
**[⬆ back to top](#table-of-contents)**

### Listing All Tickets
**[⬆ back to top](#table-of-contents)**

### Linking to Wildcard Routes
**[⬆ back to top](#table-of-contents)**

### Creating an Order
**[⬆ back to top](#table-of-contents)**

### Programmatic Navigation to Wildcard Routes
**[⬆ back to top](#table-of-contents)**

### The Expiration Timer
**[⬆ back to top](#table-of-contents)**

### Displaying the Expiration
**[⬆ back to top](#table-of-contents)**

### Showing a Stripe Payment Form
**[⬆ back to top](#table-of-contents)**

### Configuring Stripe
**[⬆ back to top](#table-of-contents)**

### Test Credit Card Numbers
**[⬆ back to top](#table-of-contents)**

### Paying for an Order
**[⬆ back to top](#table-of-contents)**

### Filtering Reserved Tickets
**[⬆ back to top](#table-of-contents)**

### Header Links
**[⬆ back to top](#table-of-contents)**

### Rendering a List of Orders
**[⬆ back to top](#table-of-contents)**
