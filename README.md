# nosql-challenge

In this challenge we were asked to undertake three parts as part of the UK Food Standard Agency's Food Hygiene evaluation program of establishments across the United Kingdom

**Part 1: Database and Jupyter Notebook Set Up**
Used the provided NoSQL_setup_starter.ipynb starter file for the following:

    * 1 - Imported data from the provided "establishments.json" file and named the database "uk_food", and the collection "establishments"
          The text used to do this: "mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json"
    * 2 - Imported the libraries "PyMongo" and Pretty Print" 
    * 3 - Created an instance of Mongo Client
    * 4 - Confirmed the database and data had been loaded properly:
            - Confirmed "uk_food" was listed
            - Confirmed "establishments" was listed
            - Displayed one document from the "establishments" collection
    * 5 - Assigned the “establishments" collection to a variable for use in Part 2

**Part 2: Update the Database**
Used the provided NoSQL_setup_starter.ipynb starter file for the following:

    * 1 - Added a new restaurant entry to the establishment collection: "Penang Flavours"
    * 2 - Identified the Business Type Id as per the new restaurant type i.e. "Restaurant/Cafe/Canteen" - returned a listing of Business ID and Type of all similar business types in the data
    * 3 - Updated the Business Type ID for the new restaurant
    * 4 - Identified and then removed all establishments from the data related to the "Dover" Local Authority and confirmed no other records were deleted
    * 5 - Updated some string values to number values including:
            - Converted Latitude and Longitude values to Decimal numbers
            - Changed non-integer values in Rating Value to null/"0" and converted all values to Integers

**Part 3: Exploratory Analysis**
Used the provided NoSQL_analysis_starter.ipynb starter file for the following:

    * 1 - Calculated the total number of establishments with a Hygiene Score equal to 20: there were 41 establishments 
    * 2 - Identified which establishments in London have Rating Value greater than or equal to 4: there were 33 establishments 
    * 3 - Identified the top 5 establishments, with a Rating Value of 5 and sorted by lowest Hygiene Score, that were within 0.01 degree of the latitude and longitude of the new restaurant
    * 4 - Identified how many establishments within each Local Authority have a Hygiene score of 0 sorting the results from highest to lowest, and identifying the top 10 Authority areas
