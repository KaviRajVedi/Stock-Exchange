# Stock-Exchange
This is the final project for CS50's Introduction to Computer Science - An introduction to the intellectual enterprises of computer science and the art of programming.  In this project, we were tasked with implementing a fully functional website for users to "buy" and "sell" stocks in a practice environment.

https://cs50.harvard.edu/x/2022/psets/9/finance/

## Overview
- Static - Contains CSS styling and any other static resources.
- Templates - HTML templates with Jinja Templating.
- application.py - Flask Application and app routes.
- finance.db - sqlite Database for logging transactions and users.
- helpers.py - Utility functions used by the APIs.

## Setup
- Clone the repository
- Install the requirements
- export FLASK_APP={directory/application.py}
- export API_KEY={IEX API Key - https://iexcloud.io/}
- flask run

## Tools
- Flask (https://flask.palletsprojects.com/en/1.1.x/)


For this project, I implemented the following functionality:

1. `register`: Allows a user to "register" on the site. The username and password are submitted via Flask and stored in a sqlite 3 database
2. `quote`: Allows a user to look up the price of a stock using the symbol
3. `buy`: Allows a user to buy the imaginary stock; Purchased stocks are saved to the database and money balance is updated
4. `index`: Displays an HTML summary table of the user's current funds and stocks
5. `sell`: Allows a user to sell stocks; Sold stocks are removed from the database and the money balance is updated
6. `history`: Displays an HTML table showing the transaction history for the user

**NOTE**: This project was completed as part of Harvard's CS50 on EdX. Requirements for this project can be found [here](https://cs50.harvard.edu/x/2020/tracks/web/finance/).   
All code outside of the above functions was provided by CS50.
