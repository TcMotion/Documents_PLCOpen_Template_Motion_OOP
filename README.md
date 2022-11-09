# Documents.
- Document versions:
    - v0.99
    - v1.0
- Library Codesys template motion OOP Axis
***
```diff
+ this text is highlighted in green
- this text is highlighted in red
```

***
```diff
PLCopen Newsletter November 2022:

To:                   Subscribers PLCopen Newsletter

Subject:           PLCopen electronic newsletter
___________________________________________________________________________
Welcome to the PLCopen® electronic newsletter.

You receive this message because you subscribed to the PLCopen electronic newsletter. 

For comments or additional information check either www.PLCopen.org or send an email to info@PLCopen.org.
___________________________________________________________________________
PLCopen Newsletter - Issue November 2022

PLCopen Application Examples for Motion Control into OOP released
________________________________________________________________________
2. PLCopen Application Examples for Motion Control into OOP released

 
With the PLCopen specification “Function blocks for Motion Control”, the PLCopen Task Force Motion Control provided a set of standardized Function Blocks to ease modularization and reuse of motion control software. 
 
We now released the document “Application Examples for Motion Control – Porting Function blocks for motion control into OOP”, version 1.0. 

This new document presents an object-oriented implementation of the motion control specification, which can be combined with the set of procedural standard Function Blocks (FBs). The general design of the proposed object-oriented (OO) implementation is a single Axis Class implementing different functions as Methods instead of formerly used multiple FBs. A benefit of the proposed software design is the compatibility with procedural motion control FBs: the standard FBs can call the Axis Class internally to combine both approaches in one application. Thus, the user of the OO implementation needs not to be familiar with the detailed OO principles or language elements for using it.

As common in object-oriented programming (OOP), an interface is used to define the motion standard since it describes how a class is presented to the outside (sometimes including the behavior). More precisely, an interface is the definition of the functionalities that a class may implement. The class is the actual implementation of the defined functionalities, including vendor-specific aspects. 

Correspondingly, this document standardizes a motion interface. For using this standard, an axis class needs to be implemented, which follows (“implements”) this standardized motion interface. In short: the interface defines the functionalities, but not how they are implemented (their content), which is done vendor-specific in an axis class.

Utilizing three application examples, this document shows how the standardized FBs from the PLCopen motion control specification can be ported to OOP by using a standardized interface itfAxis. To apply the standard in a vendor-specific implementation, the programmer develops a class, which implements the interfaces itfAxis and, thus, has all the functions standardized in itfAxis without implementation. Then the actual, vendor-specific implementation of these functions is programmed.

The advantage of the proposed interface itfAxis is that one can decide how to program: on one hand, the standard FBs can be used, and they can internally call the itfAxis methods. On the other hand, it is possible to program in OOP by using the defined methods to start a new command, get the current status of an axis, and update or abort a command. 

The details on the proposed interface and the contained methods as well as several user-defined data types are introduced in the document.

This document focuses on the motion control part of the axes only. In real projects, the axis class will have many other properties and methods for communication, hardware configuration, and additional aspects. For simplicity, these are not explained in this document.
 
The new document can be downloaded from the PLCopen website.

        plcopen_mc_application_examples_in_oop_version_1.0.pdf
```

