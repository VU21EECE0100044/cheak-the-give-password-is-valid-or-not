# cheak-the-give-password-is-valid-or-not
import re
pattern = "^.*(?=.{8,})(?=.*\d)(?=.*[a-z])(?=.*[A-Z])(?=.*[@#$%^&+=]).*$"
password = input("Enter password : ")
result = re.findall(pattern, password)
if (result):
    print ("Valid password")
else:
    print ("Password not valid")
