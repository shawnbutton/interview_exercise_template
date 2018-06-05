# Instructions

1. Please solve the following problem using `JavaScript` or `Java`
1. Avoid third party libraries with the exception of your test frameworks (i.e. Mocha/Chai, JUnit, etc).
1. Treat this problem as a library. No UI or file/console input is expected or required.
1. Add a `README.md` file that at least includes:
    - runtime versions
    - how to install any dependencies
    - how to run your tests from the command line
1. Clone this repo, and create a feature branch to work on.
1. Please commit your work regularly as you go, so we can see how you work through a problem.
1. Create a [Merge Request](https://docs.gitlab.com/ee/gitlab-basics/add-merge-request.html) into the `master` branch from your branch when you are ready for us to review your solution.
1. In the Merge Request, assign `bell-coding-exercises-integration` user as the reviewer so that we're alerted.


# Pricing Problem

We have a network of vendors who re-sell our products. We wish to provide them an application to calculate the total cost of an order.

The app needs to give volume discounts, and needs to include sales tax. 

Another system will accept input from the user, and will call this module with 3 inputs:

* number of items
* price per item
* 2-letter province code

The application should output the total price.

The total price is calculated by:

* calculate the total cost for the items
* deduct discount based on the quantity
* add sales tax based on the provice code

The following tables give the discount rate and tax rates:


## Example 1:

    Input:  $1,299.99, 3 people, food
    Output: $1,591.58

## Example 2:

    Input:  $5,432.00, 1 person, drugs
    Output: $6,199.81

## Example 3:

    Input:  $12,456.95, 4 people, books
    Output: $13,707.63
