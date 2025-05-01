# OnlineOrder

With the help of Springboot and React, we build a full stack web project about online ordering.

There'll also be GitHub Actions CI/CD pipeline involved in this project, for automated testing and deployment.

## User Requirement Design

This is a simple online ordering system that similates the process of ordering food online from different restaurants. The system allows **customers** to browse through a list of restaurants, view their menus, and place orders. The system also provides an admin interface for **restaurant owners** to manage their menus and orders.

Features:

- **Customer**:
  - Browse restaurants
  - View restaurant menus
  - Place orders in the cart
  - Customize food and delivery info
  - Pay for orders (Simulated)
  - Track order status
  - View order history
  - Cancel orders
  - Rate and review restaurants and items
  - Manage user reviews
- **Restaurant Owner**:
  - Manage restaurant information
  - Add, update, and delete menu items
  - Accept, reject, and update orders
  - Update order status
  - View order history
  - Rate and review customers
  - Manage restaurant reviews

Key points:
- The system is only simulated, and the whole process is not real.
- The restaurant owner must choose to accept or reject the order, then mark the order as available for pickup, then it will be delivered after 5 minutes. (With a 20% chance of failed delivery)
- The customer can cancel the order before it is marked as available for pickup, but not after that.
- The customer can rate and review the restaurant and the items they ordered after the order is completed and within 7 days. They cannot see the restaurant's review until they reviewed first.
- The restaurant owner can rate and review the customer after the order is completed and within 7 days. The restaurant owner can see the customer's review only after they reviewed first.
- The score for the restaurant, the items, and the customers will only calculate based on only data from 7 days ago or earlier.