# SimpleCart-2.2

***************************************************************************************								
	No databases, no programming, no headaches. A simple javascript shopping 
	cart in under 17kb that you can setup in minutes. It's lightweight, fast, 
	simple to use, and completely customizable. All you need to know is basic HTML.
  
  
*			QUICK START GUIDE														  
***************************************************************************************

* version 2.2.2: this is the last stable of release of v2.2 that uses cookies.
		
	After downloading the files, simply place a copy of the simpleCart.js 
	in your site directory, and attach it to each page that will be using the cart:
	
	1.<script type="text/javascript" src="simpleCart.js"></script>

	PayPal is the default checkout option. So if you have a Paypal account, you 
	will need to set your account email:
	
	1.<script type="text/javascript">
	2.    simpleCart.email = "you@yours.com";
	3.</script>
	
	
	----------------
	Items for Sale
	----------------

	To have an item for sale (like an awesome t-shirt), you can put it on your 
	"Shelf" like so:

	1.<div class="simpleCart_shelfItem">
	2.  <h2 class="item_name">Awesome T-Shirt</h2>
	3.  <span class="item_price">$35.95</span>
	4.  <input class="item_quantity" value="1" type="text">
	5.  <a href="javascript:;" class="item_add">Add to Cart</a>
	6.</div>

	To create a shelf item, you create a div with a class of “simpleCart_shelfItem”.
	Any field you want for your item can be set by creating a tag with a class 
	of “item_field-name” and the contents or value of the tag will be the value 
	added for the item. Please check out Shelf Setup for more info about the shelf.

	You can also add an item to the cart with a simple link:

	1.<a href="javascript:;" onclick="simpleCart.add( 'name=Awesome t-shirt' ,
	 			'price=35.95' , 'quantity=1' );">Add To Cart</a>
	
	
	---------------------------
	Cart Links and Cart Summary
	---------------------------

	If you want to display information about the cart anywhere on your page, simple 
	create any tag (div, span, a, h2, …etc) with a specific class name.

	For the total items in the cart, use “simpleCart_quantity”
	
	1.You have <span class="simpleCart_quantity"></span> items in your Cart.

	For the cart total, use “simpleCart_total”
	
	1.Cart total: <div class="simpleCart_total"></div>

	You can create a Checkout link or Empty Cart link by using "simpleCart_checkout" 
	and "simpleCart_empty"
	
	1.<a href="javascript:;" class="simpleCart_checkout">Checkout</a>
	2.<a href="javascript:;" class="simpleCart_empty">Empty</a>

	The checkout link will immediately send all the items to PayPal (or another 
	checkout option like Google Checkout) when you click it. These don't have to be 
	links, however, you can also use a div, images, or any other tag by simply 
	setting the class correctly.
	
	
	--------
	The Cart
	--------

	You can display the full cart on any page by simply creating a div with a class 
	of "simpleCart_items"
	
	1.<div class="simpleCart_items"></div>

	SimpleCart(js) will automatically populate the div with all the items in the 
	cart. You can change the appearance of your cart or what columns are in the cart 
	by checking out Cart Header Formatting.
		
		
***************************************************************************************
*	For more information, please go to simplecartjs.com								  
***************************************************************************************
