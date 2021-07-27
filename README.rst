pizzapi
=======

Description
-----------

This is a fork of https://github.com/ggrammar/pizzapi

Changes from original lib:

1. Pizza topping options from a specific store are now returned when calling `store.get_menu()`

2. Can add toppings to an order.

   `order.add_item` now takes 3 parameters:

   Code - menu item code

   Quantity - number of items desired

   Options - a dict of topping codes/quantities

   Ex::

       options = {
           #sauce, whole pizza : normal
           'X': {'1/1': '1'},
           #cheese, whole pizza  : double
           'C': {'1/1': '2'},
           #pepperoni, whole pizza : double
           'P': {'1/2': '2'},
       }

       order.add_item('P12IPAZA', 1, options)

3. Can add an integer tip when creating a payment object.

   PaymentObject(<credit_card_num>, <exp_date>, <cvv>, <zipcode>, <tip>)

   Ex::

       PaymentObject('1234567890123456', '0125', '123', '90210', '5')

4. Misc bug fixes

