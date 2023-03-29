# nosql-challenge

CSV's are imported using "mongoimport" command from Mongodb to import a collection to  a mogodb database in this case called uk_food, the collection within the database is establishments.

Using pymongo python library in the jupyter notebook file with setup_starter in its name, the establishments collection, is given a variable then:

  -the collection is updated, appending the restaurant business "Penang Flavours" to the collection and changing the business type id to match the common -   -key for Restaurant/Cafe/Canteen businesses.

  -Documents with the Dover Loval authority are removed from the collection using delete_many.

  -Latitude and longitude values are changed from strings to decimal using update_many.

In the jupyter notebook with analysis_starter in it;s name the pymongo library is also used after the establishments collection within the uk_foods database is given a variable again then the following queries are searched within the collection: 

  1. Which establishments have a hygiene score equal to 20?
  2. Which establishments in London have a RatingValue greater than or equal to 4?
  3. What are the top 5 establishments with a RatingValue rating value of '5', sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
  4. How many establishments in each Local Authority area have a hygiene score of 0?
 
 The results of these queries are pretty printed using pprint and converted to a pandas dataframe.

To run: Mongodb, Python with the libraries: pymongo and pandas. pprint should be included with the python installation. Jupyter notebook is recomnended to run the notebook files.
