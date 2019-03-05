# Mobile Development Tech Stack

## Summary

Resources for building native mobile dapps, mobile dapp browsers, and improving interoperability of mobile wallets.

Join the discussion for this resource in the [Ethereum Magicians Mobile Ring](https://ethereum-magicians.org/c/working-groups/mobile-ring)

## Tech stack options

_TODO: Add me_

## Best practices

### Managing Data

Managing data for a dApp is not your usual backend. Efficiently storing and syncing data is important.

  * Maintaining an index locally can help retrieving new data only when the user requests it.
  * Updating in the background existing data looking for new changes is always a must
  * Every request counts, don’t waste API calls for data you can retrieve once and store locally
  * Don’t forget to get the transaction count before sending a new transaction, nonces can change really fast
  * Because of the asynchronous nature of blockchains, your error handling needs to be flexible enough to cover not only hard error cases, but lack of data for subsequent requests.

### Account management

Mobile security is a different paradigm offering new solutions for common account security problems.

  * Never store private keys in plain text, encrypt them with verified and tested encryption mechanisms
  * Always empty out references in memory after signing transactions to avoid memory dumps
  * You don’t need wallet keys when reading data from the blockchain, only when sending out transactions
  * Even if the private keys are encrypted, use a secure storage mechanism client side to store the encrypted data
  * Submit all requests over secure protocols (HTTPS, etc)
  * Provide mechanisms to export/import keys securely, so clients can export their wallets to other applications, and back them up

# Placeholder content

## Features

_Main features._

### Sub-feature 1

_Content for sub-feature 1._

### Sub-feature 2

_Content for sub-feature 2._

## Resources

_Relevant resources like website, github link, blog posts etc go here_
