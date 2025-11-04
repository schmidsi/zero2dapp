# Chainlink Integration Guide

This guide will show you how to create a Token Shop to sell yout token paying with native token, sending the native token to the Token Shop address.

The token is updated to have only 2 decimal places, like fiat money, and to have AccessControl, instead of Ownable, to manage the mint permission.

- The goal is to create a TokenShop to sell the token.
- The TokenShop has a token price defined, 2usd per token.
- The user will send some amount in Eth(or native token) to the contract.
- It will use Chainlink Data Feed ETH/USD rate to calculate how many tokens the user can buy using the Eth amount sent.
- The contract will mint tokens to the user account.

