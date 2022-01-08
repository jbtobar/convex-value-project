# convex-value-project

In its current state - ConvexValue is more of a profitable proof of concept than a trailblazing business.

To grow into a trailblazing business I believe we must become a well-oiled machine composed of the following 3 branches:

 - [x] Technology
 - [ ] Operations
 - [ ] Community

***Technology***

This branch is in charge of r&d, design, building, and maintaining the ConvexValue product.

***Operations***

This branch is in charge of making sure the company itself is running smoothly. From managing finances, to handling license agreements, lawyers, to taxes, payroll, and human resources.

***Community***

This branch is in charge of sales, marketing, tutorials, customer support - and everything related to the existing and potential users of the product.


## Technology

The technological architecture of ConvexValue can be broken down into the following 5 components. Although the components speak to one another - some in more degree than others - in theory they should each be separate. What this means is that so long as the specifications of communication between one component and the other is met - whatever happens inside of the component is not the business of the other components. In practice - this means the teams behind each component can do as they wish in terms of technology stack, etc. so long as the connections are safe.

 - [ ] User accounting. (Authentication, billing, access)
 - [ ] Data
 - [ ] API
 - [ ] Modules
 - [ ] App

***User Accounting***

This means handling user account and registration (username, password), access to the platform based on payment and trial periods, connection to Stripe for payments, etc.

Works closely with `Modules` and `App` to facilitate interfaces for signup/manage account/forgot password/etc. as well as with `API` for API authentication.

***Data***

One of the most crucial components - this entails everything from receiving the data feed, processing the data, and storing the data.

Works closely with `API`.

***API***

The exposure of data and creation of data endpoints.

Works closely with `Data`.

***Modules***

This entails both the actual creation of modules and the meta (i.e - how will the architecture be of serving modules made by third parties).

Works closely with `App`, and heavily depends on `API`.

***App***

This is the actual front-end app which users interact with and in which modules are delivered.
