# Using runtime compiler 
While using runtime compiler you can either use premade scripts from our API or write your own code.

## API method
This method is really simple. You just have to run this project in visual studio, choose which premade script you want to use and click the download button. After you do so, the file you chose should be downloaded into the local directory and should move from left list to the right one. In the right list you can then select the file and after clicking load, the content of text file will be displayed in textblock above. You are free to edit the code if you want to experiment. After you are done with editing you can click the "Run" button and the code will be executed.

## Own code method
If you decided to go this way, you can start typing your code into the __.txt__ file or directly into textbox using predefined GameChar methods listed below. When you are done, save the file into the scripts/ folder located in the root directory. Then you just select your file from the list, clck "Load" and "Run".

### Methods
`GameChar.AddItem(string itemName, int itemValue);`

Adds item into the inventory list.

`string itemName` -> Text displayed in inventory

`int itemValue` -> Number of __G__ this item will be worth

`GameChar.RemoveItem(int itemIndex);`

Removes item from the inventory, character will not receive anything.

`int itemIndex` -> __ID__ of row in which this item is displayed in the inventory

`GameChar.SellItem(int itemIndex);`

Removes item from the directory, character receives Money.

`int itemIndex` -> __ID__ of row in which this item is displayed in the inventory

`GameChar.SetAttribute(string attrName, int attrValue);`

Sets chosen attribute to exact amount.

`string attrName` -> Name of the attribute you want to set.

`int attrValue` -> number you want the attribute value to be set to

`GameChar.ChangeAttributeBy(string attributeName, int changeBy);`

Changes attribute value by number.
