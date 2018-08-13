Quick Start Guide
=================

*****************************************************************************************************************************************************************************

**Creating a New Project**
==========================

*****************************************************************************************************************************************************************************
Click the Home button, and then the Add (+) button to create a new project.

Project Settings
----------------
Project Settings are a set of customizable parameters to base your design.

Default Model Parameters
------------------------
The entities or objects you will use to build your model need to have some initial or base information.  For example, to build your entire model using aluminum, select the Conductor Type from the dropdown below:

Circuit
-------
Specify the characteristics of each feeder circuit. 
For example, "Added Length" is an additional factor which is added a circuit's "Calculated Length."  Lengths are determined by equipment locations.

Calc. Settings
--------------
Specify additional calculation settings here.
For example, the Temperature Rating Threshold (NEC Table 310.15(B)) for conductors can be specified here.  The default is 110 Amps.

Auto-Sizing Filters
-------------------
Auto-Sizing Filters present designers with an option to restrict certain materials from being used in their design.
For example, if 400 kCMils are logistically not available from contractors in their region, a designer can omit this by deselecting the cable size.
Furthermore, users can also omit specific conduit sizes or breaker sizes from their design.

Flag Settings
-------------
THRUX provides code validated designs, and presents users with notifications for when their design is violating a code applicable to their project. 
Certain Flags can be ignored, or have the visibility setting omitted.

Auto-Sizing Settings
--------------------
THRUX will calculate equipment sizes automatically, but certain parameters can be excluded in the Auto-Sizing settings.  For example, if the designer would like a conduit size to remain constant or intentionally oversized to account for shaft space, deselect Conduit Size here.

*******************************************************************************************************************************************************************************************************************************************************************************************

**Defining Architectural Elements**
-----------------------------------

*******************************************************************************************************************************************************************************************************************************************************************************************

The Architectural Elements are the spacial elements which give engineers a base for their point to point calculations.  

For example, voltage drop is a calculation based on the electrical load, and the distance between the source and the load.

These elements can be created in the Floor Plans workspace, or the Architectural Elements workspace.

Floor Plans
-----------
Floor Plans are a 2-D representation of your project.  Designers can create columns and floors to build a skeleton or framework.  This skeleton can be used to model locations of equipment.  

As the architect modifies their design by changing equipment locations, THRUX designers can quickly adapt to these changes, while verifing the integrity of their design.
        
Setup Wizard
------------
Use the Setup Wizard to create the columns and floors of your project.

You can create multiple columns and floors at a time by specifying a distance in between each.  These can be individually modified in Architectural Elements.

Cycle through floors by selecting the floor on the left side bar.

Grid Editor
-----------
Use the Grid Editor to modify the spacing in between columns.

Creating Rooms
--------------
Once floors are created, create a room by hovering your mouse between column regions, and clicking Add Room.

Risers
------
Risers are shafts or spaces which are designated for groups of pipes to route to and from distribution equipment.

Therefore, instead of routing directly from a distribution equipment to a load, the route can offset through a riser shaft before terminating at the load.

To create a Riser, in the Floor Plans workspace, select a group of floors which the riser will span.  Use Shift+Click to multi-select.  Then hover over a grid region, and select Add Riser.  This can also be modified in Architectural Elements.

Load Packages
-------------
Load Packages are used to model power densities of a group of elements.  

For example, a group of floors could each have their SpaceType designated as Office, which has a specific power density.  This group of floors can be packaged as a load, and fed from a distribution equipment.

To create a Load Package, within Architectural Elements, select a group of Floors, or Rooms.  In the orange textbox, enter a name for the Load Package, and then click the (+) button.  To view your Load Packages, click the Arch. Package tab.

Load Allocations
----------------
In addition to floor or room power densities, power can be allocated to specific floors.

For example, if a designer is in the process of massing loads, and wants to assign a 50 HP load to each Office Floor, create a Load Allocation, and use the (+) button to assign it to each Floor of the Office Space Type.

*******************************************************************************************************************************************************************************************************************************************************************************************

**Building Electrical Model**
-----------------------------

*******************************************************************************************************************************************************************************************************************************************************************************************

There are 3 main workspaces to build your electrical system: One-Line, Riser, Schedules.  

The goal of these workspaces is to provide the best documentation for construction purposes, and some information is captured on multiple documents.

The locations of equipment are determined by the Architectural Model, or can be determined manually.

One-Line
--------------------

*******************************************************************************************************************************************************************************************************************************************************************************************
The One-Line depicts power flow in a top-to-bottom sequence.  Property Tags can be applied to assist with design or network visualization.

Add a Source
------------
Right click inside the workspace and click Add Source, then click Utility Source.

Add Equipment
-------------
Click on the Utility and the Selection Dial will display a ring of options.  Click the + button to Add Equipment.

Copy Equipment
--------------
To copy equipment, select the equipment to copy.  Click Copy or use CTRL + C to copy. The selection will highlight pink and be added to the clipboard.  Then, select the source or equipment to paste to, and click Paste or use CTRL+V.

Cut Equipment
-------------
To cut equipment, select the equipment to cut.  Click Cut or use CTRL + X to cut. The selection will highlight pink and be added to the clipboard.  Then, select the source or equipment to paste to, and click Paste or use CTRL+V.

Property Tags / Quick Views
---------------------------
Use Property Tags to view and edit specific elements of your design.  Click the tag symbol in the upper left of the workspace toolbar. Select the Voltage Drop Quick View to view preset property groupings.

Schedules
---------

*******************************************************************************************************************************************************************************************************************************************************************************************
Schedules are a tabular representation of your distribution system.  Schedules are primarily used for Distribution Boards, Switchboards, and Panelboards.  Not every piece of equipment has a dedicated schedule.  For example, end of line equipment such as motors do not have schedules.

Copy Equipment
--------------------
To copy equipment, select a circuit number to copy.  Click Copy or use CTRL + C to copy. The selection will highlight pink and be added to the clipboard.  Then, select a different circuit number on the same schedule, or on a different schedule, and click Paste or use CTRL+V.

Cut Equipment
-------------
To cut equipment, select the equipment to cut.  Click Cut or use CTRL + X to cut. The selection will highlight pink and be added to the clipboard.  Then, select the source or equipment to paste to, and click Paste or use CTRL+V.

Riser
-----

*******************************************************************************************************************************************************************************************************************************************************************************************

The Riser workspace is an elevational representation of the distribution system.  It is used to depict wiring routes as they disperse through a vertically scaling project.


Explorers / Utility Design Tools
--------------------------------

*******************************************************************************************************************************************************************************************************************************************************************************************

Properties Explorer
-------------------
The Properties Explorer displays the various properties associated with the current selection.

Identifying Design Flaws Using FlagTracker
------------------------------------------
Below is a small example showing a Utility source, a Distribution Board, and Motor, all in different room locations.  

The Voltage Drop Quick View is enabled, in addition to the Calculated Length and Manual Added Length Properties. 

Open the FlagTracker by clicking on the right explorer dock.  Note that the current list of flags is empty.  

Increase the Manual Added Length to 1000 for the circuit feeding the DB Distribution Board and note the list of current flags.

Pricing
-------
The price of the model is constantly being evaluated as the design changes.  Open the Pricing Explorer to view live cost impacts.

A tabular format can be viewed by opening the Pricing Report workspace.

Branching
---------
Designers are often tasked to study different options in order to determine the best option for the owner.  

To create a branch, open the Issuance Log on the right explorer bar.  Click the branch symbol and give the branch a name.  You can create a branch off the current model, or off of the last saved model.

Swap between branches by clicking the arrow symbols.  The current branch is noted in the top right navigation bar.  A branching map is displayed at the bottom of the Issuance Log.

In addition, designers can compare changes between branches, by using the Change Tracking workspace.

Change Tracking
---------------
To compare changes between branches, select the branch to compare against the current branch.  Select the entities to compare against, and select Refresh.  This list can be exported to .CSV (Excel).

Studies
-------
The Studies workspace is intended for use as a reporting tool.  

Designers can navigate through different study types like Voltage Drop, Short Circuit, and Loading.  Designers can also navigate to different workspaces to gain better perspective on their system.  

For example, a user can identify the cause of a voltage drop issue by navigating from the Studies workspace to the One-Line, Riser, or Floor Plans.

*******************************************************************************************************************************************************************************************************************************************************************************************


