# Shopping Cart Exercise with React Hooks

## Description
This project demonstrates the use of React Hooks to manage the state of a simple shopping cart application. The `ShoppingCart` component allows users to move items from a list of available products (`Product List`) to a shopping cart. The available stock of products and the contents of the shopping cart are managed using the `useState` hook.

## Key Features
- Users can add products to the shopping cart by clicking on a button corresponding to each product.
- The number of items in stock decreases as items are added to the shopping cart.
- The shopping cart displays all items that have been added.

## Code Snippets

The `useState` hook is used to create initial state for the stock and the cart:

```javascript
const [stock, setStock] = React.useState(availableItems);
const [cart, setCart] = React.useState([]);
```

The `moveToCart` function updates the stock and the cart states:

```javascript
const moveToCart = (e) => {
  // ...
  setStock([...newStock]);
  setCart([...cart, ...item]);
};
```

## Possible Use Cases
This example serves as a foundation for building more complex e-commerce applications with shopping cart functionality. The state management principles used here can be expanded to handle more complex states involving user authentication, order processing, etc.

## Installation and Usage

Clone the repository to your local machine. The project contains a single HTML file which you can open in a web browser to view and interact with the `ShoppingCart` component. 

## Contributions
Feel free to submit pull requests, create issues or spread the word.

## License
MIT License. See the `LICENSE` file for details.
