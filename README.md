# Whiskey Recommendation App
This app takes the information from the clustering analysis and uses it to provide recommendations based on user input. To use the app, enter a keyword into the search bar and click the search box. This will bring whiskies with 
the chosen keyword into box 1. Clicking on a whisky will reveal whiskies that were found to have similar descriptive profiles during clustering analysis. Clicking on one will show details of the whiskey's descriptive profile.
<br>
<h3>Virtual Environment and Setup</h3>
Type the following commands and run them in order:
<br>
<blockquote>
$conda create -n whiskey<br>
$conda activate whiskey<br>
$pip install numpy pandas matplotlib SQLAlchemy psycopg2 PySimpleGUI
</blockquote>

In addition to the environment you will need PostgreSQL. 


<img src="https://github.com/gspahlin/whiskey_recommender_app/blob/main/app_picture/whiskey_example.jpg">
