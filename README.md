![Duffel](https://i.imgur.com/W50QTZp.png)

# Getting started with the Duffel API

So, you're at a hackathon and want the fastest and easiest way to search and book flights? Duffel is the tool for you.

In this guide, you'll find everything you need to get started.

## Table of Contents

- [Introduction](#introduction)
- [Our airline partners](#our-airline-partners)
- [Getting started](#getting-started)
  * [Signing up](#signing-up)
  * [Creating your first access token](#creating-your-first-access-token)
- [Building your integration](#building-your-integration)
  * [First steps](#first-steps)
  * [Searching for flights](#searching-for-flights)
  * [Creating an order](#creating-an-order)
- [Help!](#help-)

## Introduction

With the Duffel API, you can search and book flights with more than 20 airlines through one simple platform.

We package up flights from all of our great airline partners into one easy to integrate REST API.

We're powered by direct connections' to airlines reservation systems, which means we get the best prices.

## Our airline partners

With Duffel, today you can book with:

* Aegean Airlines
* American Airlines
* Austrian
* British Airways
* Brussels Airlines
* Cathay Pacific
* Emirates
* Iberia
* LEVEL
* Lufthansa
* Olympic Air
* Qatar Airways
* Singapore Airlines
* SWISS
* Transavia
* United
* Virgin Atlantic
* Vueling
* WestJet

## Getting started

To use the Duffel API, you'll need to sign up for an account and then create an access token.

### Signing up

You can sign up for an account on the Duffel website - it takes about one minute.

Just head to <https://app.duffel.com/join> and enter your name, email address and password and you'll be good to go, with instant access to our sandbox.

### Creating your first access token

To create your access token, head to your [dashboard](https://app.duffel.com), click on your organisation name, then click "Developers", then "Access tokens", and then "New token".

Give your access token a name, and leave the scope as "Read write". Click the "Create token" button, and then you'll have your first token for our sandbox.

## Building your integration

### First steps

You'll find our API documentation  at <https://duffel.com/docs/api/overview/welcome>.

We'd recommend reading the ["Key Principles" section](https://duffel.com/docs/api/overview/key-principles) first to understand the most important concepts in our API.

### Searching for flights

To search for flights, you'll need to [create an offer request](https://duffel.com/docs/api/offer-requests/create-offer-request). 

An offer request describes the passengers and where and when they want to travel (in the form of a list of slices). It may also include additional filters (e.g. a particular cabin to travel in).

We'll send your search to a range of airlines, and return your offer request back to you with a series of offers.

Each offer represents a set of flights you can buy from an airline at a particular price that meet your search criteria.

Inside the offers, you'll see your slices, but now each slice will also include a list of one or more specific flights (called segments) that the airline is offering to get the passengers where they want to go.

### Creating an order 

Once you've found an offer that you want to book, you'll need to [create an order](https://duffel.com/docs/api/orders/create-order).

To do this, just pass in the ID of the offer you selected, some basic information about the passengers and your payment information. In our sandbox, you can pay using your Duffel Balance - it's unlimited 🎉

## Experimenting with the API in Postman

We've created a [Postman](https://www.postman.com/) collection to make it easy to get started with the API.

To start using it, open Postman, click "Import", then "Link", paste `` into the box and then click "Continue".

## Help!

There are three ways to get help with our API - before, during and after the hackathon:

* Drop by the `#01-apis-duffel` channel in the TravelScrum Slack
* Join our Slack at <https://slack.duffel.com>
* Send us an email at <help@duffel.com>