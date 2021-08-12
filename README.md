# Telephone Number Validator Cipher

Telephone Number Validator algorithm for the freeCodeCamp JavaScript Algorithms and Data Structures.

## What Is The Problem?

> Return `true` if the passed string looks like a valid US phone number.
>
> The user may fill out the form field any way they choose as long as it has the format of a valid US number. The following are examples of valid formats for US numbers (refer to the tests below for other variants):
>
> > 555-555-5555
> > (555)555-5555
> > (555) 555-5555
> > 555 555 5555
> > 5555555555
> > 1 555 555 5555
>
> For this challenge you will be presented with a string such as `800-692-7753` or `8oo-six427676;laskdjf`. Your job is to validate or reject the US phone number based on any combination of the formats provided above. The area code is required. If the country code is provided, you must confirm that the country code is `1`. Return `true` if the string is a valid US phone number; otherwise return `false`.

## How It Works

- The function takes a string and will use a regex to test if the string is true or false.
- First the regex checks if there is a 1 at the start and is optional, then will check if there is a space or a dash which is also optional.
- Secondly it will use a capture group which will check if there are 3 digits with or without parentheses.
- Finially the regex will check if there is space or dash which is optional followed by 3 digits, another space and dash optional check with the final 4 digits beging checked at the end.
- The regex will only work when there is a 3 digit area code with 7 digit number.
