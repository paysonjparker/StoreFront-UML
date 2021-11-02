# UML Class Diagram
[Storefront.UML.2.pdf](https://github.com/paysonjparker/StoreFront-UML/files/7457422/Storefront.UML.2.pdf)

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
* 
