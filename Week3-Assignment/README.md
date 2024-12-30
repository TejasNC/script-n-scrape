# amazon-price-tracker-python
Your task is to build a simple price tracker app using python that regularly compares the prices of your favorite stuff on amazon and sends you a customized notification email to tell you if the prices fell down.

This uses python and implements beautiful soup, smtplib, time and requests modules and libraries.

The libraries, modules and other tools referred during this task are as follows:

<h3>Send mail from your Gmail account using Python</h3>

<ul>

  <li><a href= "https://www.geeksforgeeks.org/send-mail-gmail-account-using-python/">SMTPlib Tutorial</a></li>
  <li><a href= "https://realpython.com/python-send-email/">RealPython</a></li>
  <li><a href= "https://www.freecodecamp.org/news/send-emails-using-code-4fcea9df63f/">Free Code Camp Tutorial</a></li>

</ul>

---
### Tasks

Template `price-tracker.py` has been provided to you. You have to complete the following tasks:

  1. Task 1: Line 19
  2. Task 2: Line 24
  3. Task 3: Line 114
  4. Task 4: Line 119

### Setting Gmail SMTP Password

Before following these steps, make sure that your GMail account has **2-Factor Verification** enabled

1. Navigate to [**Gmail Account: App Passwords**](https://myaccount.google.com/apppasswords?rapt=AEjHL4OrwU89dz8b1QyDNkZKucbOgm_8NKhED-dXDuExhXLP5W90VGHF1_ZT0aB_1NvwwT3bluDoJ1gxp2x0IwM_iMbPfqWSCKrMrI5IqN9HrR9tXEHld90)
2. Enter App Name of your choice
3. A password will pop-up. This will be your **SMTP Password**
4. Make sure you delete the created password once you are done using the script for <i>Security Reasons</i>

---

### Instructions To Run The Script

1. Open the folder in CMD or terminal and type `pip install -r requirements.txt`
2. Open **params.json**
3. Set **URL** to the amazon link of the product you want to track
4. Change the **Target_Price** to the price which you desire. You will recieve a mail when the price drops below this target price
5. Set the **Sender_Email** to the Gmail with which you have configured SMTP
6. Enter the **SMTP Password** in **Sender_Email_Password**
7. Find your [**user agent**](https://www.google.com/search?q=my+user+agent&oq=my+user&aqs=chrome.1.69i57j0l5.2294j1j7&sourceid=chrome&ie=UTF-8) and paste it in the **params.json** 
8. Save the file and run the script **price-tracker.py** in your terminal
9. The script will run and check the price of the product every 24 hours. If the price drops below your target price, you will recieve an email notification. You will also recieve an email if the price changes
10. To stop the script, close the terminal or press `ctrl+c` in the terminal

--- 


### Note
- This script uses GMail's SMTP server to send the email. You can use any email server to send the email.
