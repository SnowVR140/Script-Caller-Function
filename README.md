# Script-Caller-Function
Function Caller for Unity

This package is mostly deprecated, and there are VERY little use cases in which it would be useful, you're more than likely better off using Unity's event callers

HOW TO USE

Make the script you want the method to be called from
i.e.
using UnityEngine;

public class ExampleScript : MonoBehaviour
{
    void DoThing(int parameter)
    {
        Debug.Log(Parameter);
    }
}

Basically just define the function in the script and have nothing in that script call it

Take the function caller script and put it on the object you want and fill that out

When To Call definitions:

Awake: Gets called while being loaded, good for things being initialized
Start: Gets called on the first frame of the game running, good for functions relying off of other objects
OnEnable: Gets called every time the object is enabled
OnDisable: Gets called every time the object is disabled

Basically this script just calls a scripts function from a different object, which could be useful depending on the use case
