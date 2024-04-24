# Uni TimeTable Scraping

- This is purposely for own personal use to scrape the timetable from the university website and convert it into Google Calendar.

## Installation
1. Clone the repository
2. Install the required packages
```bash
pip install -r requirements.txt
```
3. Create a `.env` file in the root directory and add the following
```env
SENDER={google_calender_id}
PASSWORD={google_app_password}
RECEIVER={receiver_email}
```
To explain the above variables:
- `SENDER` is the email address of the Google Calendar Id. To find it go to the Google Calendar settings and find the Calendar Id, different calendars have different calendar ids, so make sure to use the correct calendar.
- `PASSWORD` is the app password of the Google Calendar. To get it please follow this tutorial - https://support.google.com/mail/answer/185833?hl=en
- `RECEIVER` is the email address of the receiver.

4. Create the Google Cloud Project for getting the Google Calendar API credentials. Follow this tutorial to get the `service_account.json` file and past to the project root folder by rename it with `service_account.json` - https://medium.com/iceapple-tech-talks/integration-with-google-calendar-api-using-service-account-1471e6e102c8

5. Run the script to test the functionality
```bash
python timetable_converter.py
```

