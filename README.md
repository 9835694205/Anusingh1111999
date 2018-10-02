# Anusingh1111999
this is my first code on github
#user registration system and login
users={}
choice=''
while choice !='q':
     choice=input("Do you want to register R/L :")
     if choice == 'R':
               username=input("Please enter username here")
               password=input("Enter your password")
     if username == '' :
               print("Please enter this field,not to be empty")
               choice = input("Do you want to register R/L :")
     elif password == '':
               print("Please enter this field,not to be empty")
               choice = input("Do you want to register R/L :")
     else:
        users[username] = username
        users[password] = password
        print("you registered successfully")
        print("Now you can login here")
        login = input("Hello, Enter Username")
        if login in users:
           pass = input("Now enter thw password")
            if pass != password:
               print("Password not correct")
               break
         else:
             print("You have successfully Login:")
             break
         else:
             print("You are not Registered")
         break
     
     elif choice == 'L':
         login = input("Hello, Enter Username")
         if login in users:
            pass = input("Now enter the password")
            if pass != password:
               print("Password not correct")
               break
         else:
             print("You have successfully Login:")
             break
         else:
             print("You are not Registered")
         break
