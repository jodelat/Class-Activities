# Conditional Render

In this activity we will render one of four different components based upon our component's state.

## Instructions

* Replace your application's `src` folder with [Unsolved/src](Unsolved/src) and start the React app in development mode by running `yarn start` in your terminal.

* This application uses Bootstrap, so make sure you're including the Bootstrap CSS CDN.
  
  ```html
  <link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet" />
  ```

* Navigate to [localhost:3000](http://localhost:3000) in your web browser and take a moment to study the rendered application.

  * At the top of the page there's a Bootstrap Navpills component. Whenever a nav element is clicked, the nav element goes into an "active" state. Whenever a nav item is clicked, it sets `this.state.currentPage` inside of `PortfolioContainer` to the selected navigation item.

* Now add code to `PortfolioContainer` so that depending on the currently selected page, a different component is rendered underneath the `Navpills` component. Example:

  * Render the `About` component when `this.state.currentPage === "About"`
  
  * Render the `Blog` component when `this.state.currentPage === "Blog"`

  * Render the `Contact` component when `this.state.currentPage === "Contact"`

  * Render the `Home` component when `this.state.currentPage === "Home"`

### Bonus

* Inside of `src/components/Navpills.js`, add code so that the `li` tag for the `currentPage` has the "active" class. This component receives the `currentPage` via props.

### Hints

* Refer to [React's Documentation on Conditional Rendering](https://facebook.github.io/react/docs/conditional-rendering.html) if you get stuck.

* Consider defining a method which returns a different component based on the value of `this.state.currentPage`.
