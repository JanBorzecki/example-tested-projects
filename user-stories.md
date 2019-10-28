*User Stories based on LOGIN and REGISTRATION process written in Gherkin*

### As a Student I want to sign in using in-app account so that I have access to more features.	

#### Scenario: Unsigned Student should be able to sign in using valid data 

GIVEN I'm an unsigned Student AND I'm on "Register/Sign in" screen 

WHEN I fill fields "Username" and "Password" with valid data AND click on "Sign in" button 

THEN I should have been successfully signed in AND message "Signed in" should be displayed.
	
#### Scenario: Unsigned Student should be able to see error message when tries to sign in using invalid data 
  
GIVEN I'm an unsigned Student AND I'm on "Register/Sign in" screen 
  
WHEN I fill fields "Username" or "Password" with invalid data AND click on "Sign in" button 
  
THEN error message "Incorrect username or password" should be displayed.
  
*Substories: User inputs invalid data into specific fields*

#### Scenario: Unsigned Student should be able to see error message when tries to sing in while being offline 
  
GIVEN I'm an unsigned Student AND I'm on "Register/Sign in" screen 
  
WHEN I fill fields "Username" or "Password" with valid data AND click on "Sign in" button 
  
THEN error message "Unable to sign in. Internet connection unavailable." should be displayed.

### As a Student I want to sign in using Facebook account so that sign in proccess is quicker and easier.	

#### Scenario: Unsigned Student should be able to sign in using an active Facebook account 

GIVEN I'm an unsigned Student AND I'm on "Register/Sign in" screen 

WHEN I click on "Sign in with Facebook" button AND I'm able to select my Facebook profile by clicking on it 

THEN I should have been successfully signed in AND message "Signed in" should be displayed.

*Substories: User has no Facebook account or it’s inactive on his device*

#### Scenario: Unsigned Student should be able to see error message when tries to sign in while being offline 

GIVEN I'm an unsigned Student AND I'm offline, whithout any internet connection AND I'm on "Register/Sign in" screen 

WHEN I click on "Sign in with Facebook" button AND I'm able to select my Facebook profile by clicking on it 

THEN error message "Unable to sign in. Internet connection unavailable." should be displayed.

### As a Student I want to sign in using LinkedIn account so that sign in proccess is quicker and easier.	

#### Scenario: Unsigned Student should be able to sign in using an active LinkedIn account 

GIVEN I'm an unsigned Student AND I'm on "Sign in" screen 

WHEN I click on "Sign in with LinkedIn" button AND I'm able to select my LinkedIn profile by clicking on it 

THEN I should have been successfully signed in AND message "Signed in" should be displayed.

*Substories: User has no LinkedIn account or it’s inactive on his device*

#### Scenario: Unsigned Student should be able to see error message when tries to sign in while being offline 

GIVEN I'm an unsigned Student AND I'm offline, whithout any internet connection AND I'm on "Sign in" screen 

WHEN I click on "Sign in with LinkedIn" button AND I'm able to select my LinkedIn profile by clicking on it 

THEN error message "Unable to sign in. Internet connection unavailable." should be displayed.

### As a Student I want to sign in using Google account so that sign in proccess is quicker and easier.	

#### Scenario: Unsigned Student should be able to sign in using an active Google account 

GIVEN I'm an unsigned Student AND I'm on "Register/Sign in" screen 

WHEN I click on "Sign in with Google" button AND I'm able to select my Google account by clicking on it 

THEN I should have been successfully signed in AND message "Signed in" should be displayed.

*Substories: User has no Google account or it’s inactive on his device*
	
#### Scenario: Unsigned Student should be able to see error message when tries to sign in while being offline 

GIVEN I'm an unsigned Student AND I'm offline, whithout any internet connection AND I'm on "Register/Sign in" screen

WHEN I click on "Sign in with Google" button AND I'm able to select my Google profile by clicking on it 

THEN error message "Unable to sign in. Internet connection unavailable." should be displayed.

### As a Teacher I want to sign in using in-app account so that I have access to all features.	

#### Scenario: Unsigned Teacher should be able to sign in using valid data 

GIVEN I'm an unsigned Teacher AND I'm on "Register/Sign in" screen 

WHEN I fill fields "Username" and "Password" with valid data AND click on "Sign in" button 

THEN I should have been successfully signed in AND message "Signed in" should be displayed.

#### Scenario: Unsigned Teacher should be able to see error message when tries to sign in using invalid data 

GIVEN I'm an unsigned Teacher AND I'm on "Register/Sign in" screen 

WHEN I fill fields "Username" or "Password" with invalid data AND click on "Sign in" button 

THEN error message "Incorrect username or password" should be displayed.

*Substories: User inputs invalid data into specific fields*

#### Scenario: Unsigned Teacher should be able to see error message when tries to sing in while being offline 

GIVEN I'm an unsigned Teacher AND I'm on "Register/Sign in" screen 

WHEN I fill fields "Username" or "Password" with valid data AND click on "Sign in" button 

THEN error message "Unable to sign in. Internet connection unavailable." should be displayed.

### As a unregistered user I want to register new account in-app so that I have access to more features.	

#### Scenario: Unregistered user should be able to register using valid data 

GIVEN I'm an unregistered user AND I'm on "Register/Sign in" screen 

WHEN I click on "Register" button AND select „Student” from „Register as:” list AND be moved to registration form AND correctly fill all mandatory fields (Email address, Full name, Password, Phone number, Date of birth with valid data AND press „Submit” button 

THEN I should have been successfully registered AND message "Registered successfully" should be displayed.

#### Scenario: Unregistered user should be able to see error message when tries to register using invalid data

GIVEN I'm an unregistered user AND I'm on "Register/Sign in" screen 

WHEN I click on "Register" button AND select „Student” from „Register as:” list AND be moved to registration form AND incorrectly fill all mandatory fields (Email address, Full name, Password, Phone number, Date of birth with invalid data AND press „Submit” button 

THEN error message "Please make sure all required fields are filled out correctly." should be displayed.

*Substories: User inputs invalid data into specific fields*

#### Scenario: Unregistered user should be able to see error message when tries to register while being offline 

GIVEN I'm an unregistered user AND I'm on "Register/Sign in" screen 

WHEN I click on "Register" button AND select „Student” from „Register as:” list AND be moved to registration form AND correctly fill all mandatory fields (Email address, Full name, Password, Phone number, Date of birth with valid data AND press „Submit” button 

THEN error message "Unable to register. Internet connection unavailable." should be displayed.

### As a unregistered user I want to register using existing Facebook account so that register proccess is quicker and easier that way.

#### Scenario: Unregistered user should be able to register in using existing Facebook account 

GIVEN I'm an unregistered user AND I'm on "Register/Sign in" screen 

WHEN I click on "Register" button AND select „Student” from „Register as:” list AND be moved to registration form AND I click on "Register with Facebook" button AND I'm able to select my Facebook profile by clicking on it 

THEN I should have been successfully registered AND message "Registered successfully" should be displayed.

*Substories: User has no Facebook account or it’s inactive on his device*

#### Scenario: Unregistered user should be able to see error message when tries to register while being offline 

GIVEN I'm an unregistered user AND I'm on "Register/Sign in" screen 

WHEN I click on "Register" button AND select „Student” from „Register as:” list AND be moved to registration form AND I click on "Register with Facebook" button AND I'm able to select my Facebook profile by clicking on it 

THEN error message "Unable to register. Internet connection unavailable." should be displayed.

### As a unregistered user I want to register using existing LinkedIn account so that register proccess is quicker and easier that way.	

#### Scenario: Unregistered user should be able to register using existing LinkedIn account 

GIVEN I'm an unregistered user AND I'm on "Register/Sign in" screen 

WHEN I click on "Register" button AND select „Student” from „Register as:” list AND be moved to registration form AND I click on "Register with LinkedIn" button AND I'm able to select my LinkedIn profile by clicking on it 

THEN I should have been successfully registered AND message "Registered successfully" should be displayed.

*Substories: User has no LinkedIn account or it’s inactive on his device*

#### Scenario: Unregistered user should be able to see error message when tries to register while being offline 

GIVEN I'm an unregistered user AND I'm on "Register/Sign in" screen 

WHEN I click on "Register" button AND select „Student” from „Register as:” list AND be moved to registration form AND I click on "Register with LinkedIn" button AND I'm able to select my LinkedIn profile by clicking on it 

THEN error message "Unable to register. Internet connection unavailable." should be displayed.

### As a unregistered user I want to register using existing Google account so that register proccess is quicker and easier that way.	

#### Scenario: Unregistered user should be able to register using existing Google account 

GIVEN I'm an unregistered user AND I'm on "Register/Sign in" screen 

WHEN I click on "Register" button AND select „Student” from „Register as:” list AND be moved to registration form AND I click on "Register with Google" button AND I'm able to select my Google profile by clicking on it 

THEN I should have been successfully registered AND message "Registered successfully" should be displayed.

*Substories: User has no Google account or it’s inactive on his device*

#### Scenario: Unregistered user should be able to see error message when tries to register while being offline 

GIVEN I'm an unregistered user AND I'm on "Register/Sign in" screen 

WHEN I click on "Register" button AND select „Student” from „Register as:” list AND be moved to registration form AND I click on "Register with Google" button AND I'm able to select my Google profile by clicking on it 

THEN error message "Unable to register. Internet connection unavailable." should be displayed.

### As a unregistered user I want to register new account in-app so that I have access to all features as a Teacher.	

#### Scenario: Unregistered user should be able to register using valid data 

GIVEN I'm an unregistered user AND I'm on "Register/Sign in" screen 

WHEN I click on "Register" button AND select „Teacher” from „Register as:” list AND be moved to registration form AND correctly fill all mandatory fields (Email address, Full name, Password, Phone number, Date of birth with valid data AND press „Submit” button 

THEN I should have been successfully registered AND message "Registered successfully" should be displayed.

#### Scenario: Unregistered user should be able to see error message when tries to register using invalid data 

GIVEN I'm an unregistered user AND I'm on "Register/Sign in" screen 

WHEN I click on "Register" button AND select „Teacher” from „Register as:” list AND be moved to registration form AND incorrectly fill all mandatory fields (Email address, Full name, Password, Phone number, Date of birth with invalid data AND press „Submit” button 

THEN error message "Please make sure all required fields are filled out correctly." should be displayed.

*Substories: User inputs invalid data into specific fields*
