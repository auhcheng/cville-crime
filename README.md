# cville-crime
ML4VA project for CS 4774 at UVA



## To do

1. Clean `Crime_Data.csv`
   1. Get latitude and longitude coordinates for each data point
   2. Convert string representation of date and time to numerical (like minutes since the first entry of the dataset)
   3. Group offenses into actual categories like arson, theft, etc.
2. Clean `Arrests`
   1. Get latitude and longitude coordinates for each data point
   2. Convert string representation of date and time to numerical (like minutes since first entry of dataset)
   3. Group statutes/offenses: regex or maybe something to do with statute number?
3. Once all cleaned, make combined dataset if possible (might be hard bc duplicates), otherwise cluster each dataset individually. Should have features:
   1. Longitude
   2. Latitude
   3. One-hot encoding for general offense categories
   4. Time
4. Other ideas
   1. Arrests could cluster with race, sex too
   2. Could try to assign a measure of wealth by location
   3. May need to filter out non-criminal/unimportant offenses like Assist Citizen, Misc, Fraud
   4. `Arrests` often has multiple offenses per arrestee, maybe should combine these offenses to get a dataset of arrestees