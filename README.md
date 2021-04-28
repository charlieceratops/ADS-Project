# Places To Go
Places To Go is the result of a group project for the subject Algorithms and Data Structures at IE University and is being developed by Manuel Concepción, Tom Frerèux-Sanchez, Carlos González and Sophie Monga. The product consists of an application that allows users to store information about places/locations they find interesting and notifies them whenever those places are inside a range defined by the user. Version 0 of the product makes use of Hash Tables, Weighted Graphs and Greedy Algorithms to build a mock-up map and a simulation of how the notification, place-saving and other functions would work.

##INSTALLATION
Download the code and upload it to Google Collaboratory or a Jupyter Notebook.

##USAGE
The first section creates a simulated map through a Weighted Graph, where the data structures called Places serve as Nodes and the Streets serve as Edges. We have created up to 63 different locations labeled as loc_number, that number being between 101 and 163 (i.e.: location 55 is loc_155). Aftert that we create the different Streets that are supposed to connect the nodes as streetnumber1_number2, representing the starting and ending location (i.e.: street45_1 means that such street connects loc_145 and loc_101). Finally, we associate each Place with the Stree(s) stemming from it. Notice that this is an Undirected Weighted Graph, and so each Street has a "copy" to stem from the ending Place (i.e.: street45_1 will be associated with loc_145, whilst street 1_45 will be associated with loc_101). Execute all the necessary cells to build the map.

The second section creates a User class with all necessary methods for the Minimum Viable Product of the app. The only necessary attribute to create the user is the username. All the other attributes, except for "saved_places" have to be defined after the user is created. The class includes a method to Save a Location (addLocation), show one/all saved locations (showALocation/showAllLocations), notify the user if they are near of a saved location (notify) and find the users' friends if they are in the range of the location (find_friends). Run the User Class, and complete the spaces we provide to create your user and their friends. After this, we can already play with Version 0.1 of Places To Go!

Run the method addLocation to the user and save as many places as you like. Then, run the methods showAllLocations and showALocation to see all/a saved place(s). For showALocation, make sure to introduce the exact same name of one of the places you introduced, otherwise, the method won't be able to find the location. Use the output of showAllLocations as a guide for these names.

Run the notify function to see which places that were saved are near the user. To change the notification range or the user's current location, change the attribute distance_notif when defining the user. The method will output the saved places in the range in ascending order of distance from the user's current location.

Run the find_friends method to see which friends are near the user. To change their range or the user's current location, change the attribute distance_notif when defining the users. The method will output the friends in the range in ascending order of distance from the user's current location.

