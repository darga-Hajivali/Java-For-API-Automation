# HashSet in API Automation

## Technologies used

-Java 17
-Maven
-Eclipse
-GitHub

----------

#1. What is HashSet?

HashSet is a class in Java Collection Framework.
used to store unique values.
HashSet doesn't allow duplicate data.
In API Automation, HashSet is useful when API response should contain only unique values.

---------

#2. Why I Use HashSet in API Automation

while testing APIs, sometimes response data contains duplicate records.
HashSet helps remove duplicate values automatically.

I can use HashSet for:

- Unique employee IDs
- Unique email validation
- Duplicate response validation
- Data comparison

---------

#3. Real-Time API Example

...Json

{
  "employeeIds": [101, 102, 103, 101]
}

Using HashSet, Duplicate values can be remove easily.

---------

#4. Java program Example 

  HashSet<Integer> employeeIds = new HashSet<>();

        employeeIds.add(101);
        employeeIds.add(102);
        employeeIds.add(103);

 System.out.println(employeeIds);

---------

#5. My Learning

I understand that HashSet is useful for validating unique API response data.
It Autmatically remove duplicate values.

---------

#6. Console Output

![Console Output] (hashset-output.png)

---------

#7. Real Framework Usage

In API Automation Frameworks, HashSet can be used for:

- Duplicate record Validation
- Unique response validation
- Data Comprision
- API Response Filtering

---------

#8. Common Mistakes

- Expecting Insertion order
- Using HashSet when duplicates are needed
- Not validating empty responses

---------

#9.  Summary

- HashSet store unique values
- Duplicate values are removed automatically
- Useful for API response validation
- commonly used in Framework utilities

---------
