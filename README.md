# Prompt  

## If you have any questions, concerns, or need anything at all please do not hesitate to contact tpuckett@diesellaptops.com

> You have 3 days to work on this project.  
> This is not pass / fail Your program will be assessed for how you go about solving the problem.  
> Not completing the challenge is not an automatic disqualification.  
> This should be written in an Object Oriented mentality.  
> This program does not need a GUI and is acceptable as a command line / terminal application  
> This program should ensure only valid data can be given when prompting user for input.

## Overview
You are creating a program that emulates the real estate purchasing process.  
The user will input an annual income, and your program will return a maximum loan pre-approval quote.  
Once the user has a pre-approval quote the user should be prompted for their minimum requirements for their house,  (sqft, bed rooms, bathrooms)
once the requirements are gathered and approved, the user should be presented with a random number of listings  
that fit their buying description. After the user chooses a home to purchase they will be given  
and overview of their payment schedule.

## Instructions

* [Gather Income](#gather-income-data)
* [Generate Maximum Loan](#generate-maximum-loan)
    * [Loan Restrictions](#loan-restrictions)
* [Gather Buyers Requirements](#gather-buyers-requirements)
* [Generate House Listings](#generate-house-listings)
  * [Listing Restrictions](#listings-restrictions)
* [Purchase A Property](#purchase-a-property)
* [Generate Bill Breakdown](#generate-bill-breakdown)

### Gather Income data
First the user should be greeted, and prompted to give their annual income. 

### Generate Maximum Loan

Once the income is recieved the user should be given a maximum loan amount.  
The maximum loan amount is generated by ensuring ***the loan will be paid off in exactly 30 years***.  
***The loan's maximum monthly payment will be 1/3 of the users monthly income,***
* 50% of the monthly payment will be used to pay down the loan amount.
* 30% of the monthly payment will be taken as interest.
* 20% of the monthly payment will be used to pay the taxes and insurance.

### Loan restrictions
> A loan cannot be less than $50,000  

When calculating the users maximum loan,  
you should not grant the user a loan if the calculated maximum loan is less than $50,000

### Gather buyers requirements
Once the user has recieved a loan pre-approval quote, the user should be prompted for the following:  
* How much square footage are they looking for
* How many bedrooms
* How many bathrooms

### Generate House Listings
Once the user has entered in that information,  
the user should be given back a list of houses that match their descriptions within their loan amount.
The list should show each houses purchase price, square footage, price per square feet, bedroom & bathroom count.

#### Listings Restrictions
> There are restrictions to what should return results  

* A house cannot have less that 250 square feet  
* A house cannot have a price less than $50,000
* The square footage of a house cannot be more than 1.25% of the houses price
* A house cannot have more than 1 bedroom per 400 square feet
* A house cannot have more than 1 bathroom per room

#### Listings Specifications

> Each house should have custom generated values.  

When generating a list of houses, there should be some where between 2 and 12 options  
unless the users requirements cause any of the restrictions to be true.  

When generating a list of houses the purchase price generated should be marked up or discounted  
depending on the number of houses in the list up to a maximum of 10%.  
For example:  
* a list of 2 houses means that the price of each house should be marked up by 10%
* a list of 7 houses means that the price of each house should be marked up by 0%
* a list of 12 houses means that the price of each house should be discounted by 10%


### Purchase a property
The user should be able to select a house from the list to purchase  
or generate a new list.

### Generate Bill Breakdown
Once a user selects a property, they should be given a break down of  
their monthly bill & amounts paid over the lifetime of the mortgage.
This should display the following information:  
#### Loan lifetime information 
* Total amount paid over the lifetime of the mortgage
* amount paid on the balance over the lifetime of the mortgage
* amount of interest paid over the lifetime of the mortgage
* amount of taxes & insurance paid over the lifetime of the mortgage  
#### Loan monthly information
* Total monthly payment.
* amount being applied to balance each month
* amount of interest paid each month
* amount of taxes & insurance paid each month
