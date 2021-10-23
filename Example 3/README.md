# Sundance-MediaPrep-SQL-Filters Example 3

Note:  Accompanying images contain redactions in order to protect sensitive information.

## Problem

######   All files within the database must be manually checked as "Ready for Air" prior to airing.  FIles that are not marked "Ready to Air" display with a warning in the broadcast automation application prior to the file airing.  The user needs to see all files in the datbase that have not been manually checked as "Ready for Air" to alleviate this issue.

## Action
  
######   In order to create a filter function that will return all files in the datbase that are not checked "Ready for Air", I need to determine what the "Ready for Air" checkbox ([Image 1](sql_filters3-1.png])) is identified as for the sake of coding the function.  A quick Google search returns that the "Ready for Air" checkbox is identified as "Misc8" in the software.  Using this, we can create a filter function that will return all files in the database that have a "NULL" value for Misc8 ([Image 2](sql_filters3-2.png)).

## Outcome

######   Using our newly created "NOT READY TO AIR" filter function, we are now able to successfully return all files within the database that have not been checked "Ready for Air" ([Image 3](sql_filters3-3.png)).

## Final Thoughts

######   Knowing that I wanted to have the function check the value of a checkbox, I initially coded this using BIT data, inputting "where Misc8 = 0" (I assumed the function would need to check for a TRUE/FALSE value).  To my surprise, this function failed when it was tested.  Having the function check for a "NULL" value gave the desired results.
