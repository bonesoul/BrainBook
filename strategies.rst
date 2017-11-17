.. _strategies:

===============
Strategies
===============

``Strategies`` are basically executed by ``The Brain Engine`` to calculated expected outcome & profit for a given set of actions. ``The Brain Engine`` can run 3 kind of strategies;

- Configuration based strategies
- Programmatic strategies
- On-the-fly strategies.

Configuration based
===================

``Configuration based strategies`` are simple ``YAML markup`` based strategies. Although it has a pretty basic syntax, it can
easly handle the most basic tasks for creating simple strategies.

.. code-block:: yaml

	name: TR markets - BTC
	description: BTC arbitrage strategy for Turkish markets
	region: TR
	author: Bonesoul
	version: 1.0
	enabled: true

	defaults:
	  input: &input 1000 TRY # default input amount

	variants:

		- name: Koinim > Paribu
		  description: Buy BTC [Koinim] > Sell BTC [Paribu]
		  exec:	
			- cashin: # Cash in TRY to Koinim.
			  - market: Koinim 
			  - amount: *input
			- buy: BTC # Buy BTC using TRY.
			- transfer: Paribu # Transfer Btc to Paribu.
			- sell: TRY # Sell BTC for TRY.
			- cashout: # Cash out TRY.	

The above strategy will basically execute these actions;

- The above strategy will basically cash in ``1000 USD`` to Bitcoin exchange called ``Koinim``.
- Will buy ``Bitcoin`` with all it's fiat.
- Transfer ``Bitcoins`` to another exchange called ``Paribu``.
- Will sell all the ``Bitcoins``.
- Will cash out from the market.