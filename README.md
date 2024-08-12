Hospital Finder Web Application
Overview
This is a Flask-based web application that allows users to search for nearby hospitals based on their current location or manually entered coordinates. Users can also search for hospitals by the disease they wish to treat. The application uses the HERE API to fetch hospital information and displays it on a simple web page.

Features
Current Location Detection: The application can detect the user's current location using the browser's geolocation feature.
Manual Location Entry: Users can manually input latitude and longitude to search for nearby hospitals.
Disease-Based Search: Users can search for hospitals based on specific diseases.
Interactive UI: The hospital list is interactive, with additional details like contact information revealed on hover.
Technologies Used
Python 3
Flask: A lightweight WSGI web application framework.
HTML/CSS: For the front-end user interface.
JavaScript: To handle geolocation and dynamic form submission.
HERE API: To fetch hospital information based on location.
Getting Started
Prerequisites
Python 3.x: Make sure Python is installed on your system.
Flask: Install Flask using pip:
bash
Copy code
pip install Flask
Requests Library: Install the requests library using pip:
bash
Copy code
pip install requests
Setup
Clone the Repository:

bash
Copy code
git clone https://github.com/kartheeii/hospital-finder.gi
cd hospital-finder
Get HERE API Key:

Sign up on HERE Developer Portal and create a project to get your API key.
Update API Key:

Replace the api_key in app.py with your HERE API key.
Run the Application:

bash
Copy code
python app.py
The application will be running at http://127.0.0.1:5000/.
Usage
Access the Application:

Open your web browser and go to http://127.0.0.1:5000/.
Search for Hospitals:

Enter your coordinates manually or click the "Get Current Location" button to automatically detect your location.
(Optional) Enter a disease name to search for hospitals specialized in that disease.
Click the "Submit" button to view the list of nearby hospitals.
View Hospital Details:

Hover over each hospital entry to view the address and contact information.
Files Structure
app.py: The main Flask application file.
templates/: Folder containing HTML templates.
index1.html: The main page where users input location and disease.
hospitals.html: Displays the list of hospitals.
static/: Folder for static files like CSS and JS (if any).
Known Issues
The application currently searches for "schools" due to a placeholder query. Change the query parameter in app.py to 'hospital' or adjust based on your requirements.
Future Improvements
Add error handling for API responses.
Implement advanced search filters.
Improve UI/UX for better user interaction.
