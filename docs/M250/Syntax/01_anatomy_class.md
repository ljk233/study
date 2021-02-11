# Anatomy of a Class

This is a brief overview of the syntax of the various features of a **concrete class** in Java, using a skeleteon strcuture. (It contains only the headers.)

## Class header

~~~java
/**
 * This is a docstring for Javadocs.
 */
public class SomeClass extends SuperClass implements AnInterface
{
    // See Variables

    // See Constructors

    // See Methods
}
~~~

## Class and instance variables

~~~java
// Class variables
private static String aClassVar = "Some text";  // class variable
private static final int aClassConst = 1;  // class constant

// Instance variables
private OtherClass ref;  // reference instance variable
private float prim;  // primitive instance variable
~~~

## Constructors

~~~java
/**
 * Zero-argument defaults constructor.
 */
public SomeClass()
{
    // Instantiate something
}

/**
 * Three-argument constructor.
 */
public SomeClass(OtherClass anObj, float aFlt, int aNum)
{
    // Instantiate something
}
~~~

## Methods

### Get methods

~~~java
/**
 * Returns the instance value of ref.
 */
public OtherClass getRef()
{
    return this.ref;
}

/**
 * Returns the instance value of prim.
 */
public float getPrim()
{
    return this.prim;
}
~~~

### Set methods

~~~java
/**
 * Sets the instance value of ref to arg aRef.
 */
public OtherClass setRef(OtherClass aRef)
{
    this.ref = aRef;
}

/**
 * Sets the instance value of prim to arg aFlt.
 */
public float setPrim(float aFlt)
{
    this.prim = aFlt;
}
~~~
