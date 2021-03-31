### SignUp form


```python
username
password
confirm password
DOB
email Id
submit
```


```python
#steps
Importing Modules
Setting up the Main Frame and layout design
Creating the Database Connection
Creating the Main Function
calling the main function

def mainloop:
{
    def username
    {
        if(username==already exist)
        print("username not available..try for another one")
       
        else:
        (get username from the input by user after validation store it in database)
    }  
    
    def password
    {
        print("password should be >=6 char & should contain 1 special char & 1 capital letter")
    
        if(password>=6 & 1 special char & 1 capital letter)  
            #call password validation funtion
            #get password from the user and after validation store it in database 
            {from getpass import getpass
            password = getpass("password: ")
            print(password)}
    
        else
            print("“Please replace with a stronger password")
    }
        
    def confirm password
         {from getpass import getpass
            confirm_password = getpass("confirm password: ")
            print(confirm_password)}
        if(password == confirm_password)
            {go for next input}
        else
            print("password and password confirmation should match")

    def DOB
        {enter DOB and store in the DB}

    def Email
     {
         if(emailid==already exist)
            print("email-id already in use..try for another one")
        
         elif(email field value is not a valid email address)
            print(“This doesn’t look like an email address. Please try again.”)
         else:
            (get email id in the input by user after validation store it in database)
         
     }
    
    
username()
password()
confirm password()
DOB()
Email()
    
    
if(username.get() == "" or
    password.get() == ""  or
    Email.get() == "")
    print("plz fill the mandatory field")

elif 
    (backend validation OK) 
    Then user creation OK and Enable Signup Submit
    
else 
    operation failure 
    
    
}

mainloop()
    
```


```python
# password validation


For example Conditions for a valid password are:

Should have at least one number.
Should have at least one uppercase and one lowercase character.
Should have at least one special symbol.
Should be between 6 to 20 characters long.

# Function to validate the password
def password_check(passwd):
      
    SpecialSym =['$', '@', '#', '%']
    val = True
      
    if len(passwd) < 6:
        print('length should be at least 6')
        val = False
          
    if len(passwd) > 20:
        print('length should be not be greater than 8')
        val = False
          
    if not any(char.isdigit() for char in passwd):
        print('Password should have at least one numeral')
        val = False
          
    if not any(char.isupper() for char in passwd):
        print('Password should have at least one uppercase letter')
        val = False
          
    if not any(char.islower() for char in passwd):
        print('Password should have at least one lowercase letter')
        val = False
          
    if not any(char in SpecialSym for char in passwd):
        print('Password should have at least one of the symbols $@#')
        val = False
    if val:
        return val
  
# Main method
def main():
    passwd = 'Tuls12@'
      
    if (password_check(passwd)):
        print("Password is valid")
    else:
        print("Invalid Password !!")
          
# Driver Code        
if __name__ == '__main__':
    main()
```

# LogIn


```python
get Username

get Password

#database verification for entered values
if (Username == EnteredUsername && Password == EnteredPassword)

Login Successful

else

Login Failed.
```


```python

```
