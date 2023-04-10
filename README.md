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
    You will need to create a Power BI report using the Power BI Desktop application or using the Power BI service. Once you have created your report, you will need to publish it to the Power BI service. You can do this by selecting the "Publish" button in the Power BI Desktop application or by selecting the "Publish" option in the Power BI service.

5. Register an application in Azure Active Directory and grant it permissions to access the Power BI REST API.
    To access the Power BI REST API, you will need to register an application in Azure Active Directory (Azure AD) and grant it permissions to access the Power BI API. Here's how to do it:

    a. Go to the Azure portal and sign in with your account.

    b. Select "Azure Active Directory" from the left-hand menu.

    c. Select "App registrations" and then select "New registration".

    d. Enter a name for your application and select "Register".

    e. Once your application has been registered, select "API permissions" from the left-hand menu.

    f. Select "Add a permission" and then select "Power BI Service" from the list of APIs.

    g. Select "Delegated permissions" and then select the "Report" permission.

    h. Select "Add permission".

    i. Select "Grant admin consent for {your tenant}" and then select "Yes" to grant permission to the application.

    j. Finally, copy the "Application (client) ID" and the "Client secret" for your application, and use them to set the POWERBI_CLIENT_ID and POWERBI_CLIENT_SECRET environment variables in your Flask application.

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