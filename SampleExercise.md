# Chapter Two: Working with Types

Union Types (Lesson 1)
===========

In the previous exercise, you extended the ```PersonalRecord``` interface by adding a new member that designates a method used to retrieve the full name of a record. In this exercise, you will create two new interfaces, ```PersonalRecordUK``` and ```PersonalRecordUSA```.

These two new interfaces will each have the following properties just like the ```PersonalRecord```:
```
- firstName

- lastName

- age

- postCode

- topThreeFoods

- getFullName(firstName: string, lastName: string)
```

The fundamental difference between the two is that the *postCode* property for the ```PersonalRecordUK``` interface will be a string while, the ```PersonalRecordUSA``` equivalent will be a number. The reason for this requirement on the *postCode* property is that postal codes in the United States of America are strictly numbers, while they are alphanumerical in the United Kingdom.

Finally, create a new type called ```UnifiedPersonalRecord``` that uses both ```PersonalRecordUSA``` & ```PersonalRecordUK``` as optional type values.

To test your solution, create two new variables, both of type ```UnifiedPersonalRecord``` and implement one of them to have a numerical postcode to match ```PersonalRecordUSA```. In contrast, the other should have an alphanumerical postcode to match ```PersonalRecordUK```.

The goal of this exercise is to use union types with interfaces to support a ```UnifiedPersonalRecord``` that supports both UK and US postal codes.
