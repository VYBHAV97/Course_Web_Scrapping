
<!-- ABOUT THE PROJECT -->
## 👨‍💻 About The Project
* Building a Web scraper for iNeuron website to get all courses information.
* Storing the scrapped data to MongoDB.
* Building a Flask App to view scrapped data.
* Deploying the app in Heroku or AWS.

<!-- USAGE -->
## ❇️ Usage
*  Web scraping is a term for various methods used to collect data from across the Internet.
*  This web scraper extracts all the data on `iNeuron website's` all course information.
*  The scrapped data is then stored to user specified Mongodb database.

<!-- STEPS -->
## 📌 Steps

* Installing Python, PyCharm, Monogodb, Git to Computer.
* Creating Flask app by importing `Flask` module.
* Getting information about iNeuron website.
* Gathering data from most static websites is a relatively straightforward process. However, **dynamic website like iNeuron**, JavaScript is used to load their content. These web pages require a different approach to collecting the desired public data.
* Scraping dynamic website using one of the most popular Python libraries, `BeautifulSoup `which can load the data into Json format by using `"script"` in `soup.find` method.

### Scraping and Inserting to DB
* With the Json data all the required data is stored into Dictionary format.
* Extracted all the course data using loops and stored as list.
* Mongodb Altas is used as DB here, with `pymongo library` mongodb is connected to python.
* Database and collections created via python and the list of dictionaries is uploaded using `collection.insert_many` method.
* Created an `app.py` to initialize

### Flask
* Importing the Flask module and creating a Flask web server from the Flask module.
* Create an object **app** in flask class with `__name__` which represents current app.py file.
* Create `/` route to render default page html.
* Create a route `/course` to get user input and if keyword is present in the Mongo DB it is shown in `results.html` page.
* Run the flask app with `app.run()` code.

