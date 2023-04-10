# powerbi-django

Power BI Report Integration with Flask
This is a simple example of how to integrate a Power BI report with a Flask web application in Python.

#   Requirements
    Power BI account
    Python 3.7 or later
    Flask web framework
    Power BI REST API client library for Python

#   Getting Started

1. Clone this repository to your local machine:

>> git clone https://github.com/thesoftcoders/powerbi-django.git

2. Create a virtual environment and activate it:
    >> python -m venv env
    >> source env/bin/activate (for Mac/Linux) or env\Scripts\activate (for Windows)


3. Install the required Python packages: 

    >> pip install -r requirements.txt

4. Create a Power BI report and publish it to the Power BI service.

5. Register an application in Azure Active Directory and grant it permissions to access the Power BI REST API.

6. Set the following environment variables:
    POWERBI_CLIENT_ID = 'your_client_id'
    POWERBI_CLIENT_SECRET='your_client_secret'
    POWERBI_SCOPE='https://analysis.windows.net/powerbi/api/.default'
    POWERBI_REPORT_ID='your_report_id'
    POWERBI_GROUP_ID='your_group_id'

7. Run the Flask application:

    >> flask run

8. Open your web browser and navigate to
    http://localhost:5000.


#   Acknowledgments
    Power BI REST API documentation
    Flask documentation
    Power BI Python client library documentation