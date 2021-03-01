---
layout: post
title:      "Rails Portfolio Project"
date:       2021-03-01 17:10:07 -0500
permalink:  rails_portfolio_project
---


### Finance

Finance is an application based on a mock brokerage firm.  When a user visits the home page all the availbel financial products are listed.  They are then able to sign up or login through github.  There are two types of users(customers or administrators).

When a customer logs in their sum of all account balances is displayed.  They can create a new account where they will choose form the availbel financial products.  A cash position for the customer is also created when an account is open.  The customer will be able to make cash deposits/withdrawls and stock purchases/sales in there account.  The customer can add/reduce shares to a current stock position.

A suer that registers as an Administrator has access to the company's financial statistics.  Customers are catorgorized into three groups: full service, standard service, and self service.  The financial stat wiew displays this info to the Administrator.

The database for Finance has tables for Users, Financial Products, User Accounts, and Positions.  Customers and Admins inherit from the Users table.  Cash and Equities inherit from the Positions table.

Future upgrades for Finance include creating a Transaction class to keep a log of crud actions within the Positions class.  The log will gather information on deposits/withdrawls and pruchases/sales.  This information will be used to display the history of the account and profits/losses from the transaction.
