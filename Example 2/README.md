# Sundance-MediaPrep-SQL-Filters Example 2

## Problem

######   The user needs to access all files in the database that have been sent to the Production department storage drive, but the current filter function does not return all files that have been sent.


## Action
  
######   Using the existing "TO PRODUCTION ONLY" filter function ([Image 1](sql_filters2-1.png)), we are able to return all files in the database that belong to the group "2PROD" ([Image 2](sql_filters2-2.png)), which returns 4 files in total.  Closer inspection of the filter function shows that it is designed to call back all files that belong to the "2PROD" group ([Image 3](sql_filters2-3.png)), but does not account for files that do not belong to the "2PROD" group (The "Group" of a file is manually assigned by the user.)  A file is automatically sent to the Production department storage drive by the database when the file ends with the characters "_2PROD".  Knowing this, we can adjust the filter function to include any files which end with those characters ([Image 4](sql_filters2-4.png)) 

## Outcome

######   Using our revised "TO PRODUCTION ONLY" filter function, we now return all files either: 
######   - in the "2PROD" group, or
######   - files with a filename ending in "_2PROD"

######   This revised filter function returns a total of 13 files ([Image 5](sql_filters2-5.png)).

## Final Thoughts

######   Because we know that the database MUST send any files ending in "_2PRDO" to the Production department storage drive, but they do not always need to belong to a group, this revision ensures that the filter function will reliably return the desired results to the user.
