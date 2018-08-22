**Frequently Asked Questions**
==============================

#######
General
#######

.. hlist::
    :columns: 1

    * Is THRUX compatible with Revit?
        Coming soon.

    * How do I see what's included in each update?
        Subscribe to our newsletter here:

    * How do I export my drawings to AutoCAD?
        Open the :doc:`Schedules <docs/userguide/buildingelectricalmodel/schedules/index-schedules>` workspace, and open the schedules you would like to export.  Click the down arrow in the top right, then click Export to AutoCAD.

        See :ref:`Exporting Schedules <Exporting-Schedules>` for more details.

    * I'm in the One-Line, how do I create equipment?
        All equipment need to have a source of power, so make sure that a source like a Utility or Generator exists first.  Right-click inside the :doc:`One-Line <docs/userguide/buildingelectricalmodel/one-line/index-one-line>`, click Add Source, then choose Utility or Generator.

        If the source is not yet defined, create an Unhosted Equipment.  Right-click inside the workspace, and then click Add Unhosted Equipment.  Use the wizard to create the equipment.

        See :ref:`Adding a Source <One-Line-Adding-A-Source>` or :ref:`Adding Equipment <One-Line-Adding-Equipment>` for examples.

    * Is there a way to create groups of equipment?
        Copying an equipment will copy all of it's downstream equipment.  Select the equipment and use CTRL+C to copy.  Then select a new source and use CTRL+V to paste.

        See :ref:`here <One-Line-Copying-Equipment>` for an example in the One-Line or :ref:`here <Schedules-Copying-Equipment>` for an example in the Schedules.

    * I've created a network, but I forgot to add a distribution board, or transfer switch, or some type of intermediate node.  How can I add this without deleting what I have?
        You have the ability to rehost circuits by dragging and dropping them from one source to another.  Simply rehost a section of your network to another source.  Then add your equipment, and reattach or feed your network from your equipment.

        See :ref:`here <One-Line-Rehosting>` for an example in the One-Line or :ref:`here <Schedules-Rehosting>` for an example in the Schedules.

    * How do I create a bus duct?
        Select an equipment.  Then select Add Equipment to create a bus duct.  

        See :ref:`here <One-Line-Bus_Duct>` for an example in the One-Line.
    
    * How do I connect a transfer switch?
        After a transfer switch is created, connect it's sources by selecting Add Equipment, and then click the Existing dropdown to select the transfer switch.

        See :ref:`here <One-Line-Transfer_Switch>` for more details.  This is also available in the Schedules workspace.

***************************************************************************************************************************************************************************************

#############
Architectural
#############

.. hlist::
    :columns: 1

    * Do I need to create the Architectural Elements or do I need to use the Floor Plans workspace?
        No.  These workspaces aid in the design process, and allow the designer to quickly alter the locations of equipment in their design, as the Architectural Elements change.  

        These workspaces aid in calculating distances between equipment, which effect point-to-point calculations.

        Though it is highly recommended, it is possible to manually enter all feeder and branch lengths.

    * I'm in the Floor Plans.  How do I create my columns and floors?
        Use the Setup Wizard to create the XGrid and YGrid (column) components, and Floors.  Use the Grid Editor to modify the columns, or manually modify these components in the Arch. Elements workspace.

        See :ref:`Floor Plans <Floor-Plans-Overview>` for more information.

***************************************************************************************************************************************************************************************

#######################
Electrical Calculations
#######################

.. _Load-Capacity:
.. _%Design-Spare-Capacity:
.. _VD%-Incoming:

.. hlist::
    :columns: 1

    * How is the length of a bus duct determined?
        A bus duct must be assigned a Room.  Every branch of the bus duct must be assigned a room.  

        Pipe and wire is used until it terminates and transitions to bus duct at the Room of the bus duct.  

        The vertical run of the bus duct is determined by the vertical distance between the Room of the branch load and Room of the bus duct.  

        The bus duct transitions to pipe and wire, and the branch circuit length is determined from the distance between the Room of the bus duct, and the Room of the load.

    * What is Load Capacity?
        Load Capacity is a custom size modified by the designer.  Protective devices are selected based on the Load Capacity.  Conductors are also selected based the Load Capacity.
        
        For example, if a designer entered 401A as the Load Capacity of a 3-ø Distribution Board, then a 600AF, 450AT breaker would be selected, fed via 3#600 kcmils phase conductors.

    * What is % Design Spare Capacity?
        % Design Spare Capacity is an adjustment factor which is based on the Code Demand Load.  

        For example, if a distribution board has a Code Demand Load of 25A, and also has a % Design Spare Capacity of 20%, the Net Load on the distribution board will read 30A.