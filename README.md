# Associate Web Engineer Assignment - Colleen E. Cash

## Requirements

- Dashboard should show a list of all applications with the ability to sort and filter
- Manager should have the ability to fave or bookmark an application for later viewing
-	Details of a specific application should be accessible
-	Use JSON data as the input for your program in place of a REST API
-	Responsive across all devices
 

## Initial Planning & Issues

I decided to use a table to display each application, while using the .getJSON method to call the data from the separate .json file that has the data of all the applicants.
All columns in the table (excluding the bookmark column) are able to be sorted ascendingly, and each table row is able to be filtered using the textbox above the table. 

I decided to use a checkbox that indicates a bookmarked listing, since the checkbox input has functionality already built that allows the box to remain checked, that way I am not loading the file up with <script> tags everywhere.

I initially wanted to have a collapsible feature that would display the applicant’s availability and answers to the questions provided, once a “see more” button/link was clicked, but I kept running into the same problem of the JavaScript string breaking and the wrong data iterating. See below for more information. I resorted to creating another table below the application listing table, that way the data is still accessible.

~~I keep getting “undefined” as an output when trying to call the questions along with the answers from the .json file.~~ Corrected the problem by removing the extra brackets located in the JSON file around the question and answer data.

In the availability section, initially I wanted to display the number output, 0, 1 and 2 as “Not Available” for 0, “AM” for 1 and “PM” for 2 but was unsuccessful. 

## Where I Struggled

### Collapsible/Nested Row for Additional Information
-	I kept running into problems with the sorting and filtering when implementing a nested row underneath the applicants main listing. But once I would sort or filter any row, it would apply to the nested row as well. 
-	Same issue occurred trying to add another row below the main rows
-	When I tried implementing the link/button that triggers a box to appear below the table with more information, all of the applicant’s extra details would appear, instead of the targeted listing clicked on.

### Pulling JSON Data from the .JSON File and into the table under the correct table headers
-	I was stuck in the beginning not understanding why the table was not distributing out underneath the respective table headers, but then went over my code again and realized I was appending the data to the wrong id and worked perfectly after correcting this issue.

## Additional Information

I was successfully able to pull up the data inside the table using Dreamweaver, but when I run the file using a web browser, the data is missing. See Dreamweaver screenshot below:

![Image](http://i64.tinypic.com/2428j9g.png)

