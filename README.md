# UML Class Diagram
![Storefront UML](https://user-images.githubusercontent.com/90354190/139885528-c0f2aa44-dd9a-4554-91be-f23e20b3bbb2.png)

# Store Front
* This is where the program is ran.
* Store Front has an inventory and shopping cart that both store Products objects stemming from the Product base class. (Weapons, Armor, and Health)
* Allows users to interact with the Store Front.

# Inventory
* Uses Polymorphism to store sub-classes (Weapon, Armor, Health) of the abstract Product base class into a sorted array list.
* Possesses the behaviors to add products to the inventory, display inventory, and to move items from the inventory to the shopping cart.
* Working on an implementation of File I/O to support saving to and reading from JSON files to insert products into the inventory.

# Cart
* Similarly to the Inventory class, uses an array list of type Product to store sub-classes of the Product base class. (Weapons, Armor, and Health)
* Possesses the behaviors to add products to the cart, display cart, and to checkout.
* Cart autmatically calculates the total price of all the products in the cart and displays that total back to the user.

# Product
* Product class is an abstarct base class that has three sub-classes that extend from it.
  * It is abstract because I do not want users to be able to create instances of it. I want them to create instances of the Product Class's sub-classes because they are much more specific and it will model the real-world.
* Each Product consists of a name, description, and price.
* Product class uses the Comparable Interface.
  * I use the Comparable Interface to override the compareTo(Product) method so that the Inventory and Cart will be sorted in the Store Front.

# Weapon, Armor, Health
* Sub-classes extending from Product base class.
* Consist of the same behaviors and characteristics as the Product class, but are able to be instantiated, unlike the Product class.
* These objects are what make up the Inventory and Cart.
