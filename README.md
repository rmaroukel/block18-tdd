# Guided Practice
```
Prompt: You were hired by a global hotel chain to redesign the functionality of the button panel on their elevators. The goal is to replace the outdated panel in over 1,200 different locations. Before you begin coding, you should make a list of all the ways these panels should be tested to make sure they are working correctly and respond to unexpected input in a way that makes sense. Remember to consider happy and unhappy paths!
```

## Happy Paths
- Push button and take us to right floor
- Right amount of buttons for each floor
- Keep track of current location
- Button light-up interaction (feedback)
- Door opening / closing button
- Emergency button / communication
- Service door/hatch


## Unhappy Paths
- Multiple buttons pressed at once (delay)
- Button doesn't work
- Taken to the wrong floor / Elevator moves in the wrong direction
- Emergency service / button not working
- Door fails to close
- Door stays open while moving


# Block 18 Workshop
```
For each prompt below: 

Read the prompt.
Identify the expectations.
Write specifications in pseudocode/plain English for all the tests that would be useful for that prompt.


Try to take any "edge cases," or unexpected circumstances, into account, and write test specs for them.
Try not to write extraneous tests!
```

## A function called "multiplication" that returns the product of the two input numbers.
- Expect `multiplying by zero` to be zero
- Expect `multiplying by a negative and a positive` to be negative
- Expect `multiplying by two negatives` to be a positive
- Expect `multiplying by a decimal` to sometimes be a decimal
- Expect `non-numbers` to be an error

## A function called "concatOdds" takes two arrays of integers as arguments. It should return a single array that only contains the odd numbers, in ascending order, from both of the arrays.
- Expect `input of both arrays with even numbers` to be message 'none found'
- Expect `input of non-numbers` to be expected output excluding non-numbers
- Expect `output` to be one array of odd integers
- Expect `outputted array` to be in ascending order
- Expect `input(s) are not arrays` to be an error
- Expect `input of duplicate integers` to be returned only once
- Expect `blank input` to be an error

## A shopping cart checkout feature that allows a user to check out as a guest (without an account), or as a logged-in user. They should be allowed to do either, but should be asked if they want to create an account or log in if they check out as a guest.
- When `a user has no account/log-in` they are given the option to sign-up
- When `a user has an account` they are able to login
- When `a guest clicks check-out` go to page for billing info
- When `an account holder clicks check-out` ask to utilize saved billing info
- When `cart is empty` an error is given with an option to continue shopping
- When `an item is added to the cart` update quantities and total price
- When `an item is removed from the cart` update quantities and total price
- When `quantity is beyond the available stock` give error to user, suggest other items
- When `user is ready to finalize order` review final item count and total price
- When `user finalizes the order` go to shipping/billing confirmation page
- When `user clicks place order` process the payment
- When `order is successful` go to order confirmation page
