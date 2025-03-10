<h1>TEXT TO SQL RETRIEVAL</h1>
<br>
<p>This project is a simple and interactive application that takes English questions as input and generates corresponding SQL queries using Google Gemini. It also executes these queries on a SQLite database and displays the results.</p>

<h3><b>Features Natural Language to SQL:</b></h3> Converts natural language questions into SQL queries using the Google Gemini generative AI model.
<h3><b>Database Integration:</b></h3> Runs generated SQL queries on a SQLite database (student.db).
<h3><b>Interactive Interface:</b> </h3>Built with Streamlit for a user-friendly, interactive experience.
<br>
<h2><b>Project Structure</b></h2>
app.py: The main application file. Contains the Streamlit interface and the logic for querying the database.
sql.py: Script to set up the SQLite database (student.db) with a STUDENT table and sample records.
Getting Started
Prerequisites
Python 3.7 or above

Install dependencies:
pip install -r requirements.txt
Set up the .env file to include your Google Gemini API key:
GOOGLE_API_KEY=your_google_api_key
Run the sql.py script to set up the SQLite database:
python sql.py
Start the Streamlit application:
streamlit run app.py
How It Works
Input your natural language question into the Streamlit app.
The app sends the question and a predefined prompt to Google Gemini.
Google Gemini generates an SQL query based on the input question. The app executes the SQL query on the STUDENT table in student.db. Results are displayed directly on the app. Example Usage Input: "How many students are in the Data Science class?" Generated SQL Query: SELECT * FROM STUDENT WHERE CLASS = 'Data Science'; Result: Displays rows matching the query.# TEXT-TO-SQL-RETRIEVAL-LLM-APP
