# Instructions

1. Please solve the following problem using `JavaScript` or `Java` (or the language of your choice).
1. Treat this problem as a library. No UI or file/console input is expected or required.
1. Provide a full suite of unit tests.
1. Add a `README.md` file that at least includes:
    - runtime versions
    - how to install any dependencies
    - how to run your tests from the command line
1. Clone this repo, and create a feature branch to work on.
1. Please commit your work regularly as you go, so we can see how you work through a problem.
1. Create a [Merge Request](https://docs.gitlab.com/ee/gitlab-basics/add-merge-request.html) into the `master` branch from your branch when you are ready for us to review your solution.


# Pricing Problem

We have a network of vendors who re-sell our products. We wish to provide them an application to calculate the total cost of an order. 

The app needs to give volume discounts and include sales tax. 

Another system will accept input from the user, and will call this component with 3 inputs:

* number of items
* price per item
* 2-letter province/state code

The application should output the total price.

The total price is calculated by:

* calculate the total cost for the items
* deduct discount based on the quantity
* add sales tax based on the province/state code

The following tables give the discount rate and tax rates:

| Order Value | Discount Rate |
| ------------- |-------------:|
| $1,000        | 3% |
| $5,000        | 5% |
| $7,000        | 7% |
| $10,000       | 10% |

| Province | Discount Rate |
| ------------- |-------------:|
| AB | 5% |
| ON | 13% |
| QC | 14.975% |
| MI | 6% |
| DE | 0% |


## Example 1:

    Input:  500 items, $1 per item, Ontario
    Output: $565.00

## Example 2:

    Input:  3600 items, $2.25 per item, Michigan
    Output: $7984.98

