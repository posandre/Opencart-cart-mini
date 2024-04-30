# Opencart-cart-mini
Advanced OpenCart 2.o mini cart module.

## Installation

1. Download the modification XML file.
2. Log in to your OpenCart admin panel.
3. Go to Extensions > Extension Installer.
4. Upload the modification XML file.
5. Go to Extensions > Modifications and click the Refresh button to apply the modification.
6. Add some changes to the file common.js
   6.1 After each line like as:
   
   ```js $('#cart-total').html(json['total']);```

   you should add this code:

   ```js $('.cart-mini-section .cart-mini-section__total-info').html(json['total_mini']);```
   
   6.2 After each line like as
   
   ```js $('#cart > ul').load('index.php?route=common/cart/info ul li');```
   
   you should add this code:

   ```js $('.cart-mini-section > ul').load('index.php?route=common/cart_mini/info ul li');```

   ## Screenshot
<img width="499" alt="image" src="https://github.com/posandre/Opencart-cart-mini/assets/45790427/36f8027c-0d27-4507-8d0a-b84702e1f285">   
