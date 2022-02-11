# UFOs

## **Data Visualization Week 11 Challenge**

### **Background**

During the Module 11, we have manage to create a webpage that offer to the UFO fans a place where they can check all the UFO Sightings with several information related to date, place, shapre and some comments of the event. This web page have also a filter capability to check the events that have occurred on a certain date.

We the challenge request we have develop new capabilites to filtered even further by more column headers. The ability to pinpoint a search by date and country, for example, would go a long way in providing more in-depth analysis of UFO sightings.

### **Objectives**
The goals of this challenge are to:

Create, update, and deploy JavaScript functions to provide additional table filters.
Update and deploy forEach (for loop) to loop through the filters and update them with user input.
Update and populate the dynamic filters and table using JavaScript and HTML.

### **Resources**
- JavaScript
- Html
- Css

### **How to use**

We have incorporated to the webpage a set of filters that allow the user to look for any criteria on the database, the procedure is quite simple:

1 - Use any or all the filteres provided according to the search parameters provided
2 - Click on the "Filter Table" bottom to display the requested search.
3 - Use the bottom "Clear Filters" to reset the table and perform a new search. 

<p align = "center">
  <img src="https://github.com/GDIAZ1106/Module_11_UFOs/blob/main/resources/filter_tutorial.png?raw=true" width="800" height="400" />
  

### **Summary**
I started by adding list items for the filters that were required (city, state, country, shape). These were added to the unordered list section in the .html file that already held the user input area for the date filter we developed in the module. Once this was completed, I built the Javascript code to grab the user input from these items and append a JS object (named "filters"). The .toLowerCase() method was useful to make sure the user input was in the correct state to match up the filters. I then found code on Stack Overflow1 that helped me remove the keys and values from the object if the user did not enter data into that field (i.e. empty value). Once we have this clean object, we can loop through it by converting the object to an array (in this case an array of key/value pair arrays) to build the filtered data. We then return to the buildTable function where we pass the filteredData as the parameter. I have also added a clear filters button and function that simply reloads the page since our default is the complete table (i.e. no filters). As a recommended action, we could improve data accuracy by creating dropdown lists for the user to choose from, but the placeholder does a pretty nice job of directing the user to the correct format for data entry.

### **References**
1. https://stackoverflow.com/questions/25421233/javascript-removing-undefined-fields-from-an-object

