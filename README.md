# UFOs

# UFO Sightings with Javascript

## Overview of Project

### Purpose

The purpose of this project is to used html and javascript to create a website where people can go and find specific UFO sightings by using multiple filters.

## Results

To get the results from the filters there was a few things that had to be done. First, created 4 more input boxes for city, state, country, and shape.

![image](https://user-images.githubusercontent.com/92827264/154873364-aed1204b-57e7-43fa-8d39-d69a693208e9.png)

Then, I had to create a d3 event listener to look at any change in my 5 input boxes. This was done by using selectAll on "input" and doing on "change" to run the update filters function. 

![image](https://user-images.githubusercontent.com/92827264/154873281-25fb32bf-ab03-4af7-bb2f-ddd1ce5736df.png)

I then created a blank dictionary variable to store my filters. After that I had to make my updateFilter function. To start I had to capture which event triggered the event listener and save the data. To do this created a variable to store the element. Then I extracted the the value of that element to a variable to be used for the filter.

![image](https://user-images.githubusercontent.com/92827264/154873717-08952fea-06c1-4fc8-961a-d0c0c8ff1026.png)

I also had to store which input id it was to a variable.

![image](https://user-images.githubusercontent.com/92827264/154873787-01c947d1-c4fa-4d6c-92f0-a6d07a150911.png)

Then I populated filters variable with the id if there is data in the value and removed it if the filter got cleared. The code is shown below.

![image](https://user-images.githubusercontent.com/92827264/154873913-2f7f4e35-3586-4e23-a025-af6fdd56db2b.png)

Then the filterTable function gets called. Which I also had to create.

To create the filterTable function I started by bringing in the original data. Then I loop through my filters variable that I am populating in the code above. When looping through the filters I am using if statements to check which arrow function I need to use to filter the data on.

![image](https://user-images.githubusercontent.com/92827264/154874274-eb3b1f28-4fe5-45b6-984c-d879e250b20e.png)

When all the filters are applied I run the build table function with the filtered data that I created.

## Summary

One draw back of this website is that it uses a specific data set. So unless someone is consistanly updating and managing this website there will not be any way to add new data to the tables.


A recommendation for this website that would help users is to have a filter for the comment section. This way if someone wants to find all events that had 4 circles.

Another recommendation is add light color to the keys. That was people can search all the instances where red lights were seen.
