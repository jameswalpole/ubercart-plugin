# Using the BitPay plugin for Drupal 6 Ubercart

## Prerequisites
You must have a BitPay merchant account to use this plugin.  It's free to [sign-up for a BitPay merchant account](https://bitpay.com/start).


## Installation

* Copy these files into sites/all/modules/ in your Drupal directory.

## Configuration

* Create an API key at https://bitpay.com by clicking My Account > API Access
  Keys > Add New API Key.
* Under Administer > Site Building > Modules, verify that the Bitpay module is
  enabled under the Ubercart - payment section.
* Under Store Administration > Configuration > Payment Settings > Payment Methods,
  enable the Bitpay payment method, and then go to the Bitpay settings menu.
* Enter your API Key under the Administrator settings dropdown menu, and enter
  other settings as desired.
* Select a transaction speed under General settings. The **high** speed will send
  a confirmation as soon as a transaction is received in the bitcoin network
  (usually a few seconds). A **medium** speed setting will typically take 10
  minutes. The **low** speed setting usually takes around 1 hour. See the
  bitpay.com merchant documentation for a full description of the transaction
  speed settings: https://bitpay.com/downloads/bitpayApi.pdf

## Usage

* When a shopper chooses the Bitcoin payment method, they will be presented with
  an order summary as the next step (prices are shown in whatever currency
  they've selected for shopping).
* Here, the shopper can either pay to the one-time-use address given, scan the
  QR code to pay, or use the Pay With Bitcoin button if they're using a
  URI-compatible wallet.

**Note:** This extension does not provide a means of automatically pulling a
current BTC exchange rate for presenting BTC prices to shoppers.
