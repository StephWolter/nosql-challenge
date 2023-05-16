# nosql-challenge
 # Use NoSQL to evaluate ratings data of establishments in the United Kingdom.

## SetUp

* Create Repository in GitHub.
[nosql-challenge repository](https://github.com/StephWolter/nosql-challenge.git)

* Clone nosql-challenge repository to personal computer, then create the folder structure:


            * Resources                     # Folder for input data
                * establishments.json       # given json data regarding UK establishments
            * NoSQL_setup.ipynb             # main code for first half of the challenge
            * NoSQL_analysis.ipynb          # main code for the second half of the challenge
            * README.md

* Examined the brief given on the bootcampspot module challenge #12 page and pulled starter files. 
* Created new Database nosql-challenge
* Pushed regularly to git repository.
* In Pandas opened given starter files.

## Part 1: Database and Jupyter Notebook Set Up

* Import establishment data and define db/collections.
    *  mongoimport --type json -d uk_food -c establishments --drop --jsonArray artifacts.json   
* Import libraries
* Create instance of Mongo
* List db, collections, and check an establishment instance.
* Call db **establishments**

## Part 2: Update the Database
* Work done in NoSQL_setup.ipynb
* Add instance to **establishments** with given data for "Penang Flavours"
* Correct the business ID to 1 for Restaurant/Cafe/Canteens.
* Remove establishments from the Dover local authority
* Correct datatypes
    * latitude/longitude to decimal128
    * ratingvalue to integer

## Part 3: Exploratory Analysis
* Work done in NoSQL_analysis.ipynb
* Question 1: Which establishments have a hygiene score equal to 20? 
    * Check how many records are available
    * Check a record to see the structure.
    * Convert to dataframe **grossest_df**
* Question 2: Which establishments in London have a Rating Value greater or equal to 4? 
    * Check how many records are available
    * Check a record to see the structure.
    * Convert to dataframe **best_df**
* Question 3: What are the top 5 establishments with a Rating Value of 5, sorted by lowest Hygiene score, 
        nearest to the new added restaurant Penang Flavours? 
    * Check how many records are available
    * Check a record to see the structure.
    * Convert to dataframe **competition_df**

## Wrote out README
* And here we are.
