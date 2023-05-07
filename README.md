Download Link: https://assignmentchef.com/product/solved-ict581-assignment-3practice-creating-a-jquery-plug-in
<br>
<strong>     </strong>

<strong> Assignment 3</strong>

in this assignment, you will practice creating a jQuery plug-in. Please check the instructions and requirements to complete this assignment.

&#x25fc; Instructions

In Assignment 3, you created a to-do list web application. In this assignment, you need to print only the list element to a pdf file—not to a browser console or HTML page. The list should be printed using a browser printing feature. Only the list items and their content should be printed; all other page elements must not be printed.

<strong><em>Tips</em></strong>: jQuery does not have the print feature, so you need to use the JavaScript print() function. Notice that the print() function does not accept any data or parameters. It can be chained to a document or window object, such as <strong><em>window.print(); </em></strong>. The best way to print just part of the page is by creating one. Here is how to create a window/document and print out using JS functions:

<ol>

 <li>Create a window using the ‘open()’ function. It’s better to use a variable so we can work on the window object later:</li>

</ol>

E.g. var print_window = window.open();

<ol start="2">

 <li>Write content to the window object using the ‘write()’ function. This function can take any type of content, but you need to pass the content as a string or DOM object. You can pass one or multiple elements, e.g. write (“content”, “div”):</li>

</ol>

E.g. print_window.document.write(“print me”)

<ol start="3">

 <li>Now, print the content using the print() function. As with the open() function, above, just chain a document/window to the print() function:</li>

</ol>

E.g. print_window.document.print();

<ol start="4">

 <li>Finally, close the window using the close() function, window.close() : E.g. print_window.close();</li>

</ol>

If you followed the steps above, you now only need to figure out how to format your content using jQuery function, then pass it to the write function. You can use this example:

<table width="0">

 <tbody>

  <tr>

   <td width="686">var print_window = window.open(); // Create a new window var world = “world”; // contentprint_window.document.write(“Hello” + ‘ ‘, world); // add content to the page print_window.print(); // print hello world print_window.close(); // close the window</td>

  </tr>

 </tbody>

</table>

<h2>Requirements</h2>

<ol>

 <li>The list elements should print <strong>under</strong> each other; not in one line.</li>

 <li>Print only the list content; not the whole DOM object.</li>

 <li>Print the list using the style listed below:</li>

</ol>

<h3></h3>

<strong>      </strong>