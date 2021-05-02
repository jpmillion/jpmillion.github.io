---
layout: post
title:      "React Redux Portfolio Project"
date:       2021-05-02 05:20:47 +0000
permalink:  react_redux_portfolio_project
---

### Ecommerce Clone

When a User visits the home page they can click a link to log in or register and also can browse the product listings.  I used the Etsy API to fetch products for the app. A User can search the trending, interesting, or all active Etsy listings.  When the User is browsing the Etsy listings if the are not logged in and click "Add To Cart" the window will alert the User to log in and the app will redirect to the log in page.  Once logged in, the User's cart will appear in the top right corner of the screen.  The cart will list the number of items currently in the cart and the total value of the items. As you add items to the cart it will update the total and number of items instantly.  The cart also displays a link to view the items in the cart.  When viewing the cart, the User can update the quantity of a specific item or remove an item from the cart. Again, the cart will update instantly.  The User can purchase the items by clicking the "purchase" button.  The cart total will reset to 0 and the cart items will be emptied. 

These are upgrades that I am planning on implementing:
* React Stripe for payments
* Order and Order Item history
* Administrative features like stats that track most sold items, most removed items from cart
* Upgrade search parameters for listings
* Display a Users recently viewed items, and associated items that other customers purchased
* OAuth
