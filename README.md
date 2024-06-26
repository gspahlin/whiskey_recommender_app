# Whiskey Recommendation App
This app takes the information from the clustering analysis and uses it to provide recommendations based on user input. This is my application to share results from the
<a href="https://github.com/gspahlin/WhiskeyAdvocate_Review_Clustering_Analysis/tree/master">Whisky Clustering Analysis</a> that I developed. The whiskey recommender app shares
insights on whiskey similarity based on the profile of descriptive words that appear in the language of the <a href="https://whiskyadvocate.com/"> Whisky Advocate</a> review elucidated
by DBSCAN clustering on vectorized reviews. The data for recommendations was scraped from WhiskyAdvocate.com in an <a href="https://github.com/gspahlin/WhiskyAdvocate_ETL">ETL process</a>
found in a separate repository. 
<br><br>
 <b>The Whisky Recommender Interface</b>
 <img src="https://github.com/gspahlin/whiskey_recommender_app/blob/main/app_picture/whiskey_example.jpg">
 <br>
<h3>Virtual Environment and Setup</h3>
Type the following commands and run them in order:
<br><br>
<blockquote>
$conda create -n whiskey<br>
$conda activate whiskey<br>
$pip install numpy 
$pip install pandas matplotlib SQLAlchemy psycopg2 PySimpleGUI
</blockquote>
In addition to the environment you will need PostgreSQL. You can download that <a href="https://www.pgadmin.org/download/">on the official website</a>. Install PostgreSQL and PGAdmin, the associated database management system.
You will then need to open PGAdmin. You should set your password and create a database called WhiskyAdvocate. Next drag whisky_db_builder.py to your Jupyter Notebooks working directory, along with the dataset folder. You will need
to suppy your database password to the script. You can do this by importing it from a custom module (as I have in my example) or more simply by declaring the password variable after the import statements, like such:
<blockquote>
password="your_password_here" 
</blockquote>
After doing this, this, you can run the database creation script and the database will be written for you.
<br>
<h3>Running The App And Explanation</h3>
Run the app by navigating to the folder with whiskey_recs_v2.py and typing the following command.
<blockquote>
$python whiskey_recs_v2.py
</blockquote>
<br>
The first time the app is run you will get a registration request from PySimpleGUI, which now requires registration, but can be registered for free for non-commercial use.
<br>
To use the app, enter a keyword into the search bar and click the search box. This will bring whiskies with 
the chosen keyword into box 1. Clicking on a whisky will reveal whiskies that were found to have similar descriptive profiles during clustering analysis. Clicking on one will show details of the whiskey's descriptive profile.
<br>
<br>
 Gregory W. Spahlinger<br>   
 gspahlin@gmail.com <br>   
 <a href = 'https://www.linkedin.com/in/gregory-spahlinger/'>LinkedIn</a>
 <br><br><br>


