# Introduction To TypeScript Course Outline

---

## Pre Prerequisites

There are a few technologies that the course assumes that a learner has some knowledge about:

- **JavaScript** (Essential): This course assumes that a learner has a working knowledge of JavaScript, at least at a basic level, but preferably at an intermediate level. You must be comfortable with concepts like `variables`, `functions`, `objects`, and `classes`.
- **Object-Orientation Concepts** (Useful but Not Required): Understanding the principles of Object-Oriented Programming (OOP) can make this course a bit easier to understand, but it is not required.
- **Operating Systems**: Windows, Linux, macOS machine.

---

## Chapter One: Introduction To TypeScript

- **Why TypeScript Exists**

  - **Learning Objectives**: The learner be able to fully grasp how TypeScript is a superset of `JavaScript` and understand the advantages of using `TypeScript` instead of `JavaScript` alone.
  - **Exercise**: This lesson does not have an exercise, as it is a soft landing that enables learners to have a basic conceptual foundation of `TypeScript`.

- **Setting Up TypeScript**

  - **Learning Objective**: Learner will be able to successfully install and set up `TypeScript` on their computer with all the required dependencies.
  - **Exercise**: Confirm the installation of the TypeScript compiler by running the command `"tsc —v"` and receiving a version number confirming that TypeScript has been successfully installed.

- **Basic TypeScript Configuration**

  - **Learning Objective**: Learner will be able to to add basic configurations for typescript projects. Configurations include setting up the desired target compilation version to be `esnext`, the output directory, and the files to be included in the TypeScript compiler's compilation scope.
  - **Exercise**: Create a new project, configure it for TypeScript usage, and set the target version of JavaScript to `ES5`. Visit [TypeScript Config](https://www.typescriptlang.org/tsconfig/) to get a full list of supported target versions.

---

## Chapter Two: Working with Types

- **Exploring Primitive Types**

  - **Learning Objectives**: Learner will leave this lesson knowing about the basic built-in types including `string`, `number`, `boolean`, `Array`, and `any`.
  - **Exercise**: Create variables for your personal profile, assigning appropriate types:

    - `firstName` (your first name)
    - `lastName` (your last name)
    - `age` (your age)
    - `topThreeFoods` (a list of your top 3 foods)
    - `isUnderSixtyFive` (flag indicating if you're under 65 years)
    - `postCode` (appropriate type for postal codes based on country)

- **Creating Custom Types**

  - **Learning Objective**: Learner will be able to create custom types using the `type` keyword and assign these newly created custom types to variables.
  - **Exercise**: Define a custom `PostCode` type for the `postCode` variable allowing it to be only numbers or strings.

- **Working with Interfaces**

  - **Learning Objective**: Learner will be able to create custom types using interfaces and assign them to objects
  - **Exercise**: Create a `PersonalInformation` interface with properties identical to the variables from previous exercise. Your new interface ensures you have more reusable and composable way to use your variables.

- **Typing Functions**

  - **Learning Objective**: Learner will be able  to assign types to function parameters and define definitions for function return types.
  - **Exercise**: Add a new member to the `PersonalInformation` interface, a method. This new method should take two parameters, `firstName` and `lastName`, and the function's signature will return a string representing the full name of a given record.

---

## Chapter Three: Advanced Types

- **Union Types**

  - **Learning Objectives**: Learner will be able to combine types and interfaces; manage variables/functions with multiple return types.
  - **Exercise**: Design multiple interfaces for UK and US-specific variations of the `PersonalRecord` interface and accommodate for country-specific differences applied to the `postcode` property.

- **Working With Enums**

  - **Learning Objectives**: Learner will be able  to define an Enum and customize the default numeric value types of Enums.
  - **Exercise**: Implement a `Gender` enum with `Female`, `Male`, and `Other`, assigning string values to each member of the `Gender` enum.

- **Implementing Generics**

  - **Learning Objectives**: Learner will be able to enable functions to use Typescript's generics feature to infer the type definition provided by developers.
  - **Exercise**: Create a function `cloneItem`, that accepts a generic type as a parameter and then makes a clone of the parameter passed. The `cloneItem` function, must return the cloned parameter, and have the same return type as the parameter passed to the function.

---

## Chapter Four: Classes & Modules

- **Defining Classes**

  - **Learning Objective**: Learner will be able to create classes in Typescript and be comfortable creating instances of classes. The learner will also learn to mutate class definitions with interfaces and inherit classes to compose complex relationships.
  - **Exercise**: Create a class `PersonalBiography`, that has three properties inside it first name, last name and date of birth.

- **Adding Access Modifiers**

  - **Learning Objective**: Learner will be able to use the `private`, `public`, `protected`, `readonly`, and `static` keywords to encapsulate or expose members of class instances.
  - **Exercise**: Update the class `PersonalBiography` and have its constructor be able to set the first name, last name and date of birth with the correct data types. Ensure that it has a `public` method that can be used to get a person's. Once an instance of `PersonalBiography` is created, the first name, last name, and date of birth should not be mutable, but can be accessed via an instance of `PersonalBiography`.

- **Defining Modules**

  - **Learning Objective**: Learner will be able to use the `import` and `export` keywords to grant access to reusable pieces of code, making it easier to organise code.
  - **Exercise**: Create a new file/file to store all the interfaces used in previous steps, and use the module scope to access them from the new file/files.

- **Global Types For Modules**

  - **Learning Objectives**: Learner will be able to create type definitions for global modules that do not have prior TypeScript implementations. The learner will also understand the concept of ambient modules and know how to handle type definition declarations for them.
  - **Exercise**:In this exercise, you are to assume that we are using a global JavaScript function called `generateSocialSecurityNumber()`. You are to assume that this new `generateSocialSecurityNumber()` function returns a 10-digit alphanumeric string as a social security number. To make your code compatible with this function, create a definition for it and ensure that TypeScript now understands how to define and handle it correctly. 
