# Goodnight-Cat-Twilio-Text
Script that sends goodnight and a cat fact to people

script reads an excel file for name and numbers, then sends a goodnight text and a cat fact to that number.
replace the following in the gnight_text.py file


accountSID = 'input your account SID Twilio'
authToken = 'Input your Auth Token Twilio'

twilioCli = Client(accountSID, authToken)
myTwilioNumber = '+input 10 digit number'
os.chdir('change to desired working directory')

file = open("catfacts.txt").readlines()
wb = openpyxl.load_workbook('twiliodb1.xlsx', use_iterators=True)
