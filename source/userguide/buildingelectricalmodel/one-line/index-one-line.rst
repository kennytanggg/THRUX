############
**One-Line**
############
The One-Line depicts power flow in a top-to-bottom sequence.  

Utility functions like navigation, or additional viewing properties can be found on the workspace toolbox at the top.  

:ref:`Property Tags <One-Line-Property_Tags>` can be applied to assist with design or network visualization.

.. index:: How to Create a Source

.. _One-Line-Adding_A_Source:

Add a Source
============

Use the Setup Wizard in the top right to create a source.

.. image:: images/one-line-create_source_1.PNG
    :align: center

Choose Create Source.

.. image:: images/one-line-create_source_2.PNG
    :align: center

.. image:: images/one-line-create_source_3.PNG
    :align: center

Or, Right-click inside the workspace, click Add Source, then click Utility Source. 

.. image:: images/one-line-create_source_4.PNG
    :align: center

.. image:: images/one-line-create_source_5.PNG
    :align: center

.. image:: images/one-line-create_source_6.PNG
    :align: center

.. _One-Line-Adding_Equipment:

Add Equipment
=============

Click on the Utility and the Selection Dial will display a ring of options.  Click the + button to Add Equipment.

.. image:: images/one-line-add_equipment.PNG
    :align: center

Select an equipment type from the New dropdown menu.  Give any new equipment a name.  In this case, specify a Load Capacity, and click Select.

.. image:: images/one-line-add_dist_board.PNG
    :align: center

.. index:: How to Copy Equipment - One-Line

.. _One-Line-Copying_Equipment:

Copy / Paste Equipment
======================

To copy equipment, select the equipment.  Click Copy or use CTRL + C to copy. The selection will highlight pink and be added to the clipboard.  

.. image:: images/one-line-copy_equipment.PNG
    :align: center

Then, select the source or equipment to paste to, and click Paste or use CTRL+V.

.. image:: images/one-line-paste_equipment.PNG
    :align: center

Delete Equipment / Delete Network
=================================

To delete equipment, select the equipment.  Then Click Delete (trash symbol) or use DEL to delete. 

.. image:: images/one-line-delete_equipment.PNG
    :align: center

If the selected equipment is feeding downstream equipment, you can either delete the selected equipment, or the entire network.

.. image:: images/one-line-delete_network.PNG
    :align: center

.. _One-Line-Rehosting:

Dragging / Rehosting Equipment
==============================

To redirect an equipment's source, click and drag the equipment from its current source, to a different source.

.. image:: images/one-line-rehost_1.PNG
    :align: center

Drop, or release the equipment on its new source.

.. image:: images/one-line-rehost_2.PNG
    :align: center

Navigate
========

Navigate grants the ability to jump between workspaces based on the current selection.

.. image:: images/one-line-navigate.PNG
    :align: center

A designer can view an equipment's schedule, location on the Riser, location on the Floor Plans, or the Studies workspace.

.. image:: images/one-line-navigate_schedules.PNG
    :align: center

View Schedule
=============

To view to an equipment's schedule, select the equipment, and then click View Schedule.

.. image:: images/one-line-view_schedule.PNG
    :align: center

Searching
=========

To search for equipment, click the magnifying glass in the top left.  Start to type the name of the equipment you are searching for.  Select the equipment, and the workspace will navigate to the associated equipment.

.. image:: images/one-line-searching.PNG
    :align: center

Settings
========

Toggle the visibility settings of OCPD's by hitting Show OCPD.

.. image:: images/one-line-ocpd_settings.PNG
    :align: center

Load Calculations
=================

Normal
------

Calculations are based on the Net Load.

Board Capacity
--------------

Calculations are based on the capacity of the board.

.. _One-Line-Load_Override:

Load Override
-------------

Calculations are based on the Load Override value.  For example, if a designer wants to model a specific loading scenario between points in their distribution system, enter these loading values into Load Override.

.. _One-Line-Property_Tags:

Property Tags / Quick Views
===========================

Use Property Tags to view and edit specific elements of your design.  Click the tag symbol in the upper left of the workspace toolbar.  

Quick Views are preset property groupings such as Voltage Drop, Loading, Load Diversification, and Circuit Routing. 

.. image:: images/one-line-property_tags_quick_views.PNG
    :align: center

Expanding / Collapsing Equipment
================================

Sections of the distribution network can be expanded or collapsed on an individual or group basis.  An alternative to expanding equipment is by double-clicking on the node.

.. image:: images/one-line-expand_collapse.PNG
    :align: center

One-Line View Selectors
=======================

Different Views can be applied to aid the designer.  

By default, Normal is selected.  

Isolated Systems is recommended when viewing transfer switches.  The designer can study voltage drop as a switch is fed from different sources.

Load Flow is recommended when studying how a system is loaded.

.. image:: images/one-line-load_flow.PNG
    :align: center

.. _One-Line-Transfer_Switch:

Creating a Transfer Switch
==========================

Transfer switches are connected to a primary and secondary source of power.  To create a transfer switch, click Add Equipment, and choose ATS/STS.

.. image:: images/one-line-transfer_switch_1.PNG
    :align: center

.. image:: images/one-line-transfer_switch_2.PNG
    :align: center

To connect the secondary source of power, choose another distribution equipment.  Then click Add Equipment, and select an ATS/STS from the Existing dropdown menu.

.. image:: images/one-line-transfer_switch_3.PNG
    :align: center

.. _One-Line-Bus_Duct:

Bus Duct
========

Select an equipment.  Then select Add Equipment to create a bus duct.  

.. image:: images/one-line-bus_duct_1.PNG
    :align: center

.. _One-Line-SCC:

Short Circuit Current - SCC
===========================

Select the Utility source.  Under the "Miscellaneous" property grouping, enter the value under Available SCC (kA).

.. image:: images/one-line-SCC.PNG
    :align: center

.. _One-Line-Tap:

Bus Node
========

To model a tap, create a Bus Node in between the source and the load.

.. image:: images/one-line-tap_1.PNG
    :align: center

.. image:: images/one-line-tap_2.PNG
    :align: center
