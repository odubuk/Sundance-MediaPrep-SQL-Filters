# Sundance-MediaPrep-SQL-Filters

##Description:

Sundance MediaPrep features the ability to create content filters which allows the user to access content within the database that matches specific criteria.  Examples of these labels include "Movies", and "Commercials", and more. 

For example, a user can use the "Movies" filter to have the application only show files labelled as "Movies", or files labelled as "Commercials".
  
This repository contains visual examples of filters I have developed, as well accompanying README's which detail different elements specific to each content filter.


##FAQ:

-   What is Sundance MediaPrep?

  Sundance MediaPrep is an application developed by Sundance Digital for broadcast automation which allows the user to control the ingesting (recording) of material into a digital video server, manage the server and automation databases, and process traffic logs.
  
  
-   How do you use MediaPrep in your work environment?

  In my job as a master control operator, my fellow operators & I use MediaPrep on a daily basis to access all of our media files in order to prepare said files for our broadcast automation systems.  These media files number in the tens of thousands, containing various types of media (from commercials to 30 minute shows, to feature length films, and more).  The media files are organized using a predetermined ID system of cart numbers which are constantly rotating and being reused (e.g. one cart number may be assigned to a specific file for a specific amount of time before the file is destroyed, upon which the cart number is reassigned to another file).
  
  One aspect of our role as a master control operator is the management and cleaning of the data within the database.  Because cart numbers & file ID's are constantly rotating in & out of usage, we are responsible for ensuring that all data is accurate and that storage capacity is as large as it possibly can be.  This requires regular purging of outdated content within the database to ensure that there is room for new content as it is ingested into the server.
  

-   What was your reasoning for development of these filters?

  The MediaPrep application comes with prebuilt filters, such as the aforementioned "Movies" and "Commercials", which work on a general use level but are not tailored to an individual entity's usage of the application.  Each television station is different, and has different needs and ways of managing content on their digital video server(s).  With regards to the station I work at, we have a small team of users who work with MediaPrep, and each of those individuals has a varying degree of knowledge with respects to the application itself as well as computers/IT in general.
  
  My goals in the development of these filters were as follows:
  
  - Create filter functions which solve problems that the preexisting filters do not address.
  - Create filter functions which help the user to achieve a desired goal regardless of their expertise/understanding of the MediaPrep application.
  - Perform quality assurance testing on developed filter functions to ensure that they produce the desired results.

  More specific information pertaining to each example can be found in the example's accompanying README file.
