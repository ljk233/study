# Messages in Java

A **message** is a request for an object to do something.
The only way to make an object do something is to send it a message.
The set of messages that an object can understand is set out in its protocol.
The *behaviour* of an object is its response to the messages in its *protocol*.

A message may:

1. change the state of an object
2. make an object do something without changing its state
3. get back some useful information from an object
4. cause an object to send a message to another object
5. cause an object to send a message to itself

## Terminology

**Message answer**
: A message answer is an object's reply to a message.
Not all messages elicit a message-answer (this can be checked by looking at the return type in the corresponding method signature).

**Message expression**
: A message-send that evaluates to some value, i.e. the message returns a message answer.
We also say that it *returns a value.*

**Message name**
: The name of a message, including the following parentheses, but excluding any arguments.

**Message-send**
: The code that sends a message to an object.
If a message requires no arguments, then the message-send is the same as the message name.

## Arguments

**Actual arguments**
: An actual argument is a value used in a message that is copied to a formal argument for use inside the corresponding method.
Actual arguments must be of a compatible type with their corresponding formal arguments.

**Formal arguments**
: A typed identifier used in a method signature between parentheses to stand for a value (an actual argument) that is passed into the method body by a message.
This is the argument used when implementing the method.

## Getter and setter messages

It is common for the protocol of an object to include a pair of message that either return or set the value of an attribute.

**Getter message**
: A message that returns as its message answer the value of one of the receiver’s attributes.

**Setter message**
: A message that sets the value of one of a receiver’s attributes.

## Example

If a method was implemented as follows

~~~java
public void setName(String aName)
{
    // do something
}
~~~

Then

- There would be no message answer, as the return type is `void`
- This is not a message expression, because the message returns to no answer
- Its message name would be `setName()`
- A message send would be `anOject.setName("Joe Bloggs")`

The formal argument of the method would be `aName`.
An actual argument could be `"Joe Bloggs"`.
