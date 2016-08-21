# CSC1401-Assignment-2
CSC1401 Foundation Programming Assignment

# Operation of the Program
As the prototype for a web-based shopping cart system, the program is to be implemented in
JavaScript and running on F irefox, an operating system independent web browser. HomewareCity
has specified the following business requirements:
1. The program should be running without errors throughout two Phases: Information Gathering
and Information Presenting.

2. In Information Gathering, each time the user adds one product item to the shopping cart.
The program should first confirm with the user for willingness of shopping before proceeding
to gather information of the product item in purchase.

3. When receiving an order, the program should first prompt and ask the user to enter the
product code before adding the product item to the shopping cart. If the user enters an
invalid value, for example, a non-number value or a non-existing product code, the program
should alert an error message on screen and then prompt the user for re-enter. The process
should iterate until a valid product code is entered.

4. If the entered product code is valid, the program should then prompt the user to input the
quantity value in purchase. Again, if an invalid value is input, such as a non-number value,
a negative number or zero, the program should display an error message then iterate until
receive a valid number for quantity.

5. After valid input of product code and quantity, the program should add the product item
into the shopping cart, and then loop back to seek user confirmation for either proceeding
further to add one more item or moving to the Information Presenting Phase for check-out.
6. If the user confirms not to shop anymore, the Information Gathering Phase is completed and
the program then moves to Information Presenting.

7. In the Information Presenting Phase, the program prints on the web page a table containing
the product items in the shopping cart, including information such as product names, prices,
quantity, and cost.

8. To make the Shopping Cart System user-friendly, HomewareCity also expects the program
to display some statistic information:
i.    The total amount for ordered items in the shopping cart;
ii.   The average cost per item in the cart;
iii.  The most expensive product item;
iv.   The least expensive product item.

# Requirements Requirements
These requirements are in conjunction to the steps above.

You need to create two arrays – one to store the product code of ordered products (namely
orderedP roductCodeArr), the other to store the quantity of ordered products (namely quantityArr).
Just like productListArr and priceListArr, an ordered products’ code and quantity will be stored
at exactly the same index in their corresponding arrays.

1. In the beginning of the program, print to a table the catalogue for all products including name,
code, and price, to assist users shopping. You should use a loop plan to access the data stored in
productListArr and priceListArr and present it in a four-column table, like Figure 4, where each
column is a set of products with code, name, and price.

2. You need to implement a validation plan to get a valid input from the user for product code. An
input value is considered invalid if:
i. it is not a number at all;
ii.   it is not an integer number;
iii.  it is a negative number;
iv.   it is a number out of range (greater than or equal to the size of productListArr).

3. You need to implement another validation plan to get a valid input from the user for quantity. An
input value is considered invalid if:
i.    it is not a number at all;
ii.   it is not an integer number;
iii.  it is zero or a negative number;
iv.   it is greater than 100.

4. You need to design a looping plan to implement the Information Gathering Phase. Refer to Functional
Requirements and Fig. 1 for the detail of data flow in the loop. Clearly, this task should
incorporate the works in Task 2 and 3.

5. Your program needs to calculate the total cost for all ordered products in the shopping cart. The
calculation formula is provided: 

![alt tag](https://i.imgur.com/omlUchO.jpg)

6. Your program needs to find the most expensive product in the shopping cart. To do it, for each of the
products added in to the cart you need to retrieve the corresponding price from priceListArr, and
then compare the prices one by one. Once you find out the most expensive price, the corresponding
product item in productListArr will be the most expensive product in the shopping cart.
If you have multiple products in the cart sharing the same most expensive price you can select any
one of them as the “most expensive product”.

7. Your program also needs to find the least expensive product in the shopping cart. You may adopt
the the same strategy in previous task for this task. Again, if you have multiple products in the
cart sharing the same least expensive price you can select any one of them as the “least expensive
product”.

8. Your program needs to be able to calculate the average cost for all product items in the shopping
cart. This can be done by the total cost divided by the accumulated value of quantities:

![alt tag](https://i.imgur.com/e7aBaLp.jpg)

You should handle the “Division by Zero” exception when calculating average.

9. Print to a table the detailed information of shopping cart, such as product name, price, quantity,
and cost. You should adopt an iteration plan to visit the elements stored in quantityArr and
orderedP roductCodeArr in order to get the index to retrieve product names and prices from
productListArr and priceListArr.
All currency values should be at cents in terms of precision.

10. Print to an unordered list the statistic information (total cost, most expensive item, least expensive
item, and average cost per unit for the ordered product items) on shopping cart.
The table and the list should be formatted like the screenshot in Figure 2. The same as that in
Task 9, all currency values should be at cents in terms of precision.

# Optional Requirements - No extra marks given
HomewareCity will appreciate it if an extra feature can be delivered to detect duplicate orders. If
an ordered item has already been in the cart, the system should detect it, and then ask for user
confirmation for updating the quantity or not. If the user gives a positive confirmation, the system
will proceed to prompt for quantity and then replace the stored quantity by the newly entered
value; otherwise, the program terminates the current product-adding process and loop back to ask
user confirmation for adding a new item or not. Note that the user is not allowed to completely
remove an ordered item from the shopping cart.


# Testing
You need to test the program for all functionality thoroughly before delivering the program. The
program should be running appropriately without any syntax and logic errors.

# Non-Functional Requirements
i. All code should appear in the script section in the head of the HTML document. Do not
write any code in the HTML body. All functionality are delivered by JavaScript.
ii. In the script order your code as follows:
(a) Constants;
(b) Variables and objects (declared and initialised);
(c) Other statements.

iii. Variable and constant identifiers should use an appropriate convention. Identifiers should be
written consistently throughout the code.
iv. Code is indented appropriately and grouped in blocks according to the common tasks attempting
to.
v. Appropriate comments should be added to all blocks of code. Do not simply translate the
syntax into English for comments, instead, describe the purpose of the code block.

# Submission
A team makes only one common submission, in which all members should make equal
contributions and share the same mark.

For a complete submission you need to submit two files as specified below. You can submit them
individually or compress them into a .zip (or .rar ) file and submit it. The assignment submission
system will accept only the files with the extensions specified in this section.

1. Statement of Completeness in a file saved in .doc, .docx, .odt, .rtf or .txt format in 200-300
of your own words describes the following issues. You should first specify the registered name
of the team and all members’ name and student ID on the top of the statement.

i. The state of your assignment, such as, any known functionality that has not been
implemented, etc. (It is expected that most teams will implement all of the functionality
of this assignment.)

ii. Problems encountered, such as, any problems that you encountered during the assignment
work and how you dealt with them. This may include technical problems in
programming and people-soft problems in team working;

iii. Reflection, such as, any lessons learnt in doing the assignment and handling teamworking
and suggestions to future programming projects.

2. The program in a file saved with an .html extension contains the source code implemented
following the functional and non-functional requirements.

