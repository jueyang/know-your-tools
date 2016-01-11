### Get data

Get **DOHMH New York City Restaurant Inspection Results** from [NYC OpenData](https://nycopendata.socrata.com/). Okay, to save you one second for this workshop, here's the [link](https://data.cityofnewyork.us/Health/DOHMH-New-York-City-Restaurant-Inspection-Results/xx67-kt59).

### Create a work space using command line:

1. Make a directory called "commmandandcontrol" on your desktop
2. Move the csv file you exported from the above link to the new directory

### The investigation begins:

1. Back up
  	- `cp`, tab completion
2. Rename the file more sensibly
    - `mv`
3. How big is the file?
    - `ls -l`
4. What is the file about?
    - `head`
5. But I want to look at this in Excel because it's prettier there.
    - Alright, as you wish. Create a new file with only the first few lines of the file. hint: `>`
6. Search for records that contain "mice" and create a new file
    - `grep -iw`
7. Now look at the file again. Notice something? Right. How to deal with multiple records for one place.