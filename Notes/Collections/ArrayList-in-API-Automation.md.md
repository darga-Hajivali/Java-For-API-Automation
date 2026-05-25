## ArrayList in API Automation

##Technologies Used
-Java 17
-Rest Assured
-Maven
-Eclipse

----
#1. What is ArrayList?

ArrayList is used to store dynamic data in Java.

In API Automation, we can use ArrayList to store:

user Ids
employee names
API endpoints
response values

ArrayList is useful when API response contain multuple Records.
----

#2. Why I use ArrayList in API Automation

while practicing Rest Assured APIs, I noticed many responses return multiple values.

Examples:

multiple user IDs
list of emails
employee records

ArrayList helps store and validate this dynamic response data easily.

----

#3. Realistic API-Style Example

,,,,json

{
  "employeeIds": [201, 202, 203]
}
,,,,,

or

,,,,json

{
  "emails": [
    "testuser1@gmail.com",
    "testuser2@gmail.com"
  ]
}

,,,,

----

#4. My Learning

I understood that ArrayList is very useful when API responses return multiple records.
I can use it in Rest Assured to store responses value and validate data later.

----

#5. Console Output
![Console Output](arraylist-output.png)

----

#6. Issue Faced 

Initially, I got 401 Unauthorized error becuase the API Key header was missing.
Later, I recived a 403 Forbiddden error due to an invalid API Key.
I fixed the issue by using the complete APII Key correctly.

#7. Fix

Added x-api-key header correctly in Rest Assured request.

----

#8. Real Framework  Usage
 
In Real API Automation Frameworks, ArrayList can be used for:

Storing multiple response IDs
Validating duplicate records.
Storing endpoint lists.
Dynamic payload validation.

----
#9. Mini Summary

ArrayList stores dynamic data
useful for handling API responses
Help validate multiple records
Commonly used in Rest Assured framework

----