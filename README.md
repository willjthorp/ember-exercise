## Task Description

You are the lead FE programmer for a small web shop. You are required to make a simple
page where the user can add products to a cart, and the total of the cart is updated
in real time.

#### API

You will have an API endpoint that returns products with the following structure (assume
your preferred seralization format)

| id      |  name        | price  |
| ------- | :----------: | :----: |
| GR1     |  Green tea   | £3.11  |
| SR1     | Strawberries | £5.00  |
| CF1     |    Coffee    | £11.23 |

There will be an API endpoint to actually do the checkout, charge customer etc, but it won't 
be used here.

## Special conditions:

- The CEO is a big fan of buy-one-get-one-free offers and of green tea. He wants us to add a
rule to do this.
- The COO, though, likes low prices and wants people buying strawberries to get a price
discount for bulk purchases. If you buy 3 or more strawberries, the price should drop to £4.50
- The CTO is a coffee addict. If you buy 3 or more coffees, the price of all coffees should drop
to two thirds of the original price.

We can assume that discount do not change very often so they can be hardcoded in the
application, for display purpose.

Our check-out can scan items in any order, and because the C\*Os change their minds, it needs 
to be flexible regarding our pricing rules.

## Deliverables:

- A view where the user can add items to the basket
- A component that displays the total amount of the basket (discounts applied)
- A service or similar that is responsible of calculating said total amount

The application must be demoable without an actual backend (use some approriate
client-side API server for demoing)
