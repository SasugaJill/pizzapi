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

 - Misc bug fixes

