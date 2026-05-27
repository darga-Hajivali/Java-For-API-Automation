#1. What is HashMap?

HashMap is a class in Java Collections Framework.
It stores data in Key-Value format.
In API Automation, HashMap is commonly used to create request payload dynamically.

For Instance:
firstname --> Darga
Lastname --> Hajivali

-------

#2. Why we use HasMap in API Automation

while practicing Rest Assured APIs, I noticed most APIs use Json requests bodies.
HashMap helps create dynamic payload data easily.

we can use HashMap for:

- Request payload creation
- Query Parameter
- Headers
- Dynamic Test Data
- Response validation

-------

#3. Real Time Payload Example

example API request body

,,Json

{
  "firstname": "Darga",
  "lastname": "Hajivali",
  "email": "darga@gmail.com",
  "job": "API Automation Engineer"
}

This Payload can be created dynamically using HashMap.

-------

#4. Java program

package com.api.payloads;

import java.util.HashMap;

public class HashMapPayloadExample {

    public static void main(String[] args) {

        // Creating HashMap for API payload
        HashMap<String, Object> payload =
                new HashMap<>();

        // Adding request body data
        payload.put("firstname", "Darga");
        payload.put("lastname", "Tester");
        payload.put("email", "darga@gmail.com");
        payload.put("job", "API Automation Engineer");

        // Printing Payload
        System.out.println(payload);
    }
}

-------

#5. Rest Assured Usage

,,,JAVA

given()
.body(payload)
.when()
.post("/users");

In Rest Assured Frameworks, HashMap can be directly passed as request body.

-------

#6 My Learning 

I understand that HashMap is very useful for API payload handling.
It helps create request body data dynamically instaed of writing large Json Strings Manually.

-------
#7 Real Framework Usage

In Real API Automation Frameworks, HashMap is used for:

- Dynamic Payload creation
- Storing request parameters
- Managing Headers
- Handling Test Data
- API request Customization

-------

#8 Mistakes

- Using wrong key names
- Adding null values without validation
- Storing Incorrect Data Types
- Hardcoding payload values everywhere
- Not validating payload before request execution

-------

#9 Summary

- HashMap stores data in Key-value format
- widely used in API Payload handling
- Help create dynamic request bodies
- commonly used in Rest Assured frameworks

-------