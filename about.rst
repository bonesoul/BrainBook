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




CoiniumServ is an platform-agnostic software which can run on any platform that dotNet_ or mono_ framework is available including Windows, Linux and Mac/OS.

* Windows: dotNet_ v4.5+.
* Linux: mono_ v3.2+.
* MacOS over mono_ v3.2+.

Once you do have either .net / mono installed, you can then run CoiniumServ. You have basically two options; compiling from source or using a binary distribution.

Binary Distribution
===================

Our binary distributions can work on any platform including Windows, Linux and MacOS. You can purchase a binary distribution over `here <http://www.coiniumserv.com/shop/releases/coiniumserv/>`_ to support the project.

.. image:: http://i.imgur.com/MDYxtOO.png

Once you download the package, extract the contents to a suitable folder. Then you can simply run the **CoiniumServ.exe**

.. image:: http://i.imgur.com/MhJkZxT.png

Then you have to configure the server to get it working.

Compiling from source
=====================

If you like you can get the sources of the project and compile yourself.

  * Windows_
  * Linux_
  * MacOS_
  
Then you have to configure the server to get it working.

.. _Mono: http://www.mono-project.com/
.. _dotNet: http://www.microsoft.com/net
.. _Windows: https://github.com/CoiniumServ/CoiniumServ/wiki/Getting-Started:-Windows
.. _Linux: https://github.com/CoiniumServ/CoiniumServ/wiki/Getting-Started:-Linux
.. _MacOS: https://github.com/CoiniumServ/CoiniumServ/wiki/Getting-Started:-MacOS
