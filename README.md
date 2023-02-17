<h1>Cold Call Assistant</h1>
Cold Call Assistant is an open-source application developed using the Frappe Framework, Twilio API, OpenAI's GPT-3 API, Whisper API, and Google Text-to-Speech API. The application automates the process of cold calling potential leads and guiding them through a scripted conversation to generate pre-set targets, such as obtaining email details or scheduling an appointment. The results of each cold call are displayed within the application, and any targets generated during the conversation are highlighted in the interface.

Getting Started
These instructions will help you set up the project on your local machine for development and testing purposes.

Prerequisites
Python 3 and pip
A Twilio account with an active phone number
An OpenAI API key
A Whisper API account
A Google Cloud Platform account with an active project and Text-to-Speech API enabled
Installing
Clone the repository to your local machine using Git.

Navigate to the root folder of the project and create a virtual environment:

Copy code
python3 -m venv venv
Activate the virtual environment:

bash
Copy code
source venv/bin/activate
Install the required packages:

Copy code
pip install -r requirements.txt
Create a .env file at the root of the project with the following content:

makefile
Copy code
TWILIO_ACCOUNT_SID=your_twilio_account_sid
TWILIO_AUTH_TOKEN=your_twilio_auth_token
TWILIO_PHONE_NUMBER=your_twilio_phone_number
OPENAI_API_KEY=your_openai_api_key
WHISPER_API_KEY=your_whisper_api_key
GOOGLE_APPLICATION_CREDENTIALS=path_to_your_gcp_service_account_key_file
Replace the your_twilio_account_sid, your_twilio_auth_token, your_twilio_phone_number, your_openai_api_key, your_whisper_api_key, and path_to_your_gcp_service_account_key_file placeholders with your own credentials and file path.

Usage
Activate the virtual environment:

bash
Copy code
source venv/bin/activate
Run the application:

sql
Copy code
bench start
Open a web browser and navigate to http://localhost:8000.

Use the application to import lead details, select API service providers, and provide the base prompt for OpenAI's GPT-3 API.

Click the "Start" button to initiate a call to a lead and start a conversation with them.

Contributing
Please read CONTRIBUTING.md for details on the code of conduct, and the process for submitting pull requests.

License
This project is licensed under the GNU General Public License version 3 (GPL-3.0), which is a free and open-source software license that allows people to use, copy, modify, and distribute the code for any purpose, as long as they include the original copyright notice and disclaimer, and any modifications made to the code are also released under the GPL-3.0. The GPL-3.0 ensures that the code remains free and open-source, and that any improvements or modifications made to the code are also shared with the community.

Acknowledgments
Frappe Framework
Twilio API
