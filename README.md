## This is a repository for the Ghana Pothole Tracker system.
It runs on a raspberry pi and uses image classification methods to determine the presence of potholes on a road in realtime, and transmits the co-ordinates of said potholes to a MySQL database.
These co-ordinates are then plotted on a web application to inform user's route selection. Additionally, they are available for download.

The purpose of this project is to introduce an element of crowdsourcing for civil good in user journeys, making it easier for the mobile maintenance units (MMU's) to gather data about road improvement projects.

#Dataset
Expected input data is a folder of images, with the naming convention of the folder contents representing the image classes. eg. pothole.1.png & not_a_pothole.1.png
The full stops are necessary, as the script splits the filenames in order to get the image label.

#Usage
These files are meant to be run in the command line, with the syntax "pythonx file_name.py --dataset /path/to/dataset/here"
The output is the classification metrics and confusion matrix for the given data.

An extra script (test.py) is included to allow the user to verify the results with their own data.
