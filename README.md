Download Link: https://assignmentchef.com/product/solved-cs1520-project-3-application-of-priority-queues-in-data-structures
<br>
To explore an advanced application of priority queues in order to gain a deeper understanding of the data structure.

<h1>Background</h1>

You will be writing a basic application to help a user select a car to buy. You will write a menu-based user interface driver program (to be run in the terminal, no GUI), but most of the logic will be in implementing a priority queue-based data structure. You should write a PQ-based data structure that stores objects according to the relative priorities of two of their attributes, making it efficient to retrieve objects with the minimum value of either attribute. Your data structure should further be indexable to allow for efficient updates of entered items. You will want users to be able to enter details about cars that they are considering buying. The user should then be able to efficiently retrieve the car with the lowest mileage or lowest price. These retrievals should be possible on the set of all entered cars or on the set of all cars of a specific make and model (e.g., “lowest price Ford Fiesta”, “lowest mileage Cadillac Escalade”).

<h1>Specifications</h1>

<ol>

 <li>First you must create a class to store data about cars to buy Specifically, this class must contain the following information:</li>

</ol>

A unique VIN number: a 17-character string of numbers and capital letters, excluding I (i), O (o), or Q

(q) to avoid confusion with numerals 1 and 0

The car’s make (e.g., Ford, Toyota, Honda)

The car’s model (e.g., Fiesta, Camry, Civic)

The price to purchase (in dollars)

The mileage of the car

The color of the car

<ol start="2">

 <li>You must write a terminal menu-based driver program (again, no GUI). Specifically, your driver must present the user with the following options:

  <ol>

   <li>Add a car</li>

  </ol></li>

</ol>

This will prompt the user for each of the above-listed attributes of a car to keep track of.

<ol start="2">

 <li>Update a car</li>

</ol>

This option will prompt the user for the VIN number of a car to update, and then ask the user if they would like to update 1) the price of the car, 2) the mileage of the car, or 3) the color of the car

<ol start="3">

 <li>Remove a specific car from consideration</li>

</ol>

This option will prompt the user for the VIN number of a car to remove from the data structure (e.g., if it is no longer for sale)

Note that this mean you will need to support removal of cars other than the minimum (price or mileage) car

<ol start="4">

 <li>Retrieve the lowest price car</li>

 <li>Retrieve the lowest mileage car</li>

 <li>Retrieve the lowest price car by make and model</li>

</ol>

This option will prompt the user to enter a make followed by a model, and then return the car with the minimum price for that make and model.

<ol start="7">

 <li>Retrieve the lowest mileage car by make and model</li>

</ol>

This option will prompt the user to enter a make followed by a model, and then return the car with the minimum mileage for that make and model.

<strong>Note:</strong> Retrieval operations should <em>not</em> remove the car with minimum price or mileage from the data structure, just return information about that car. Cars should <em>only</em> be removed via the “remove a specific car from consideration” menu option.

<ol start="3">

 <li>To aid in the testing of your application, you will find an example file with some test data stored in your folder ( txt ). Your progam should read in the contents of this file to initialize your data structure each time it is run. You can assume that this file will already exist, and you do not need to write an updated version of the data structure back to the file.</li>

 <li>To ensure efficiency of operations, you must base your data structure around the use of heaps with indirection (making them indexable). Note that retrieval operations on either attribute (e.g., retrieve minimum price, retrieve minimum mileage) must have a logarithmic runtime (both for all cars and for a specific make and model). Updates and removals must also have a logarithmic runtime. Take care in selecting your approach to the indirection data structure to account for the types of keys you will need to store and the type and number operations that you will need to perform on them.</li>

 <li>Because this project requires you to make a number of decisions about how to implement its requirements, write a documentation file explaining your implementation and <strong>justifying your decisions</strong>. Name this file txt . Be sure to document your approach carefully, to reduce the effort required to trace through your code for grading. State the runtime and space requirements of your approach, and use this information as part of your explanation of why you chose your approach.</li>

</ol>