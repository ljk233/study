# Classes, Objects, and Attributes

## Objects

**A general description of an object and its relationship with its class.**

## Attributes

### Attributes and instance variables

It is common that there is one-to-one relationship between an attribute and some instance variable, but it is not neccessarily the case.

!!! example
    A person has a **first name** and **last name.**  These are attributes we could implement using two instance variables: `fName` and `lname`.
    But a person also has another attribute: **full name,** which we would not implement in this case, instead we would write a getter method `getFullName` that would return both the `fName` and `lName` instance variables.

    That way, if we wish to change how a person's full name is represented, we would only need to change the one method.

### Attributes and state

Reference: *U01, SAQ 2*

Attributes describe the kind of information that can be determined about an object.
The state of an object is the particular data held by all the attributes at a given time.

## Keywords

**Attribute**
: Some property or characteristic of an object that can be accessed using a getter method.
Attributes are generally implemented by instance variables.
An object's attributes are defined by its class.

**Class**
: A class is a blueprint for the creation of objects.
They ensures that all its instances have the same instance variables and behave in response to messages in an identical manner.

**Instance variable**
: A variable whose identifier and type is common to all the instances of a class, but whose value is specific to each instance.
Each instance variable either contains a reference to an object or contains a value of some primitive type.

**State**
: The values of the attributes of an object constitute its state.
The state of an object can vary over time as the values of its attributes change.
