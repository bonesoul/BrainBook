.. _gettingstarted:

===============
About
===============

Why?
====

As trading hundreds of cryptocoins in tens of markets could be really hard for users, The Brain aims to help with decision taking by presenting the user best possible summarized information.

How?
====

The Brain consists of multiple parts for use; The UI and Engine. The Brain Engine is responsible for running everything behind the curtain including reading & analyzing
market data and processing it with opportunity analyzers & strategies.

Market Data
===========

Brain can read market data from hundres of possible cryptocoin exchanges. Yet again
users can also develop their own market data reader programmatically and The Brain will be then executing it.

Yet again, The Brain can read from fiat conversion API's available through the web to
execute cross-fiat conversions.

Data Analyzers
==============

Once the market data from all available sources are read, The Brain Engine will then
will start executing the available data-analyzer modules.

A data-analyzer is a basic module that can read, process and finally manipulate the data from markets.

As an example "MergedMarketsForPairs" data-analyzer merges all currency pairs within the market data and will then find each market with best ask & bid prices.