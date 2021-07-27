pizzapi
=======

Description
-----------

This is a fork of https://github.com/ggrammar/pizzapi

Changes from original lib:

 - Pizza topping options from a specific store are now returned when calling store.get_menu()

 - Can add toppings to an order.
   order.add_item now takes 3 parameters:
   Code - menu item code
   Quantity - number of items desired
   Toppings - a str of topping codes

   Ex: order.add_item('P12IPAZA', 1, 'J=1,N=1')

 - Can add an integer tip when creating a payment object.
   PaymentObject(<credit_card_num>, <exp_date>, <cvv>, <zipcode>, <tip>)

   Ex: PaymentObject('1234567890123456', '0125', '123', '90210', '5')

 - Misc bug fixes

