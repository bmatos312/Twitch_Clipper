Twitch Clip & YouTube Uploader
This application automates the creation of Twitch clips based on chat intensity and uploads them to YouTube. It integrates Twitch and YouTube APIs to create, download, and upload Twitch clips as YouTube Shorts, allowing streamers to highlight important moments from their streams.

Features
Chat Intensity Monitoring: Automatically triggers clip creation when chat activity reaches a specified threshold.
Twitch Clip Creation: Generates Twitch clips when chat activity is high, based on the chat message rate.
YouTube Upload: Downloads the created clips and uploads them to YouTube as videos.
Credential Management: Users can securely input and save their Twitch and YouTube API credentials via a simple GUI interface.
Installation (Using the Executable)
You don't need to install Python or any additional dependencies. Simply download the provided .exe file and run it directly on your machine.

1. Download the Executable
Download the .exe file from here. (Provide a link to your .exe file upload, such as a Google Drive or Dropbox link).
Save it to a directory on your computer.
2. Run the Application
Once you have downloaded the executable:

Double-click the .exe file to start the application.
The first time you run it, a GUI window will appear where you can enter your Twitch and YouTube credentials.
3. Input Your API Credentials
You’ll be prompted to enter your Twitch and YouTube credentials, including the Client ID, Client Secret, and Refresh Token for both APIs. These credentials are necessary to interact with the Twitch and YouTube APIs to create clips and upload them.

4. Monitor Chat and Create Clips
The application monitors Twitch chat in real-time. When the chat activity exceeds the defined threshold (i.e., the number of messages within a specified timeframe), a clip will be automatically created.

5. Customize the Clip Title
After the clip is created, the program allows you to edit the clip’s title via a simple prompt. Once you’ve set the title, the clip will be uploaded to YouTube.

6. Upload to YouTube
The application will automatically upload the created Twitch clip to YouTube with the title you provide. It uses the YouTube Data API to manage the upload process.

Configuration
The following variables can be adjusted inside the application code (not accessible from the GUI at this time):

CHAT_THRESHOLD: Number of chat messages required to trigger a clip.
THRESHOLD_SECONDS: Time frame (in seconds) to measure chat intensity.
BROADCASTER_ID: Your Twitch broadcaster ID (used to create clips).
Security
Credential Encryption: API credentials are encrypted and stored securely using the cryptography package. A secret.key file is generated to handle encryption, and this file should be kept secure to prevent unauthorized access.
Prerequisites
Even though the application is pre-compiled as an .exe, you’ll still need the following:

A Twitch Developer account with a registered app. You’ll need the Client ID, Client Secret, and an OAuth Access Token.
A YouTube API account with OAuth credentials. You’ll need the Client ID, Client Secret, and Refresh Token.
Follow the steps in the Setting Up Twitch API and Setting Up YouTube API sections below to get your credentials.

1. Setting Up Twitch API
Go to the Twitch Developer Console and create a new application.
Copy
