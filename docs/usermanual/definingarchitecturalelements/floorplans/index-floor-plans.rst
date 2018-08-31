.. _Floor-Plans:

Setup Wizard
------------

Use the Setup Wizard to create the columns and floors of your project.

.. image:: images/setup_wizard.PNG
    :align: center

You can create multiple columns and floors at a time by specifying a distance in between each.  These can be individually modified in Architectural Elements.

.. image:: images/column_creator.PNG
    :align: center

Cycle through floors by selecting the floor on the left side bar.

.. image:: images/floor_selection.PNG
    :align: center

Grid Editor
-----------

Use the Grid Editor to modify the spacing in between columns.

.. image:: images/grid_editor.PNG
    :align: center

Creating Rooms
--------------

Once floors are created, create a room by hovering your mouse between column regions, and clicking Add Room.  

.. image:: images/room_creation.PNG
    :align: center

To create a room in a common location spanning multiple floors, use Shift+Click to select multiple floors, and then hover over a grid region to click Add Room.

.. image:: images/multi_room.PNG
    :align: center

Risers
------

Risers are shafts or spaces which are designated for groups of pipes to route to and from distribution equipment.

Therefore, instead of routing directly from a distribution equipment to a load, the route can offset through a riser shaft before terminating at the load.

To create a Riser, in the Floor Plans workspace, select a group of floors which the riser will span.  Use Shift+Click to multi-select.  Then hover over a grid region, and select Add Riser.  This can also be modified in Architectural Elements.

.. image:: images/riser.PNG
    :align: center

Moving Rooms / Risers
---------------------

Once rooms or risers are created, move a room or riser by clicking and dragging it to the new region.

.. image:: images/move_room.PNG
    :align: center

Conduit Lengths
---------------

Conduit lengths are determined by a starting location, and an ending location.  

.. image:: images/conduit_lengths_1.PNG
    :align: center

The Calculated Length, or orthogonal route, between two pieces of equipment is determined by their Room locations.  A designer can modify the Manual Added Length to account for additional distance.

.. image:: images/conduit_lengths_2.PNG
    :align: center

In addition, if the conduits are being routed through a riser shaft, assign a Riser to the terminating equipment.

.. image:: images/conduit_lengths_3.PNG
    :align: center

.. _Floor-Plans-Move_Equipment:

Moving Equipment
----------------

Move Equipment is intended for designers to quickly place equipment in Rooms.  

.. image:: images/move-equipment_1.PNG
    :align: center

There are two collections of Equipment: Orphaned Equipment and Hosted Equipment.  Orphaned Equipment do not have a Room assigned to them.  Hosted Equipment are Rooms.

.. image:: images/move-equipment_2.PNG
    :align: center

Select the Equipment you would like to move.  Drag and drop it in a Room location.

.. image:: images/move-equipment_3.PNG
    :align: center

The Room indicator will notify the designer when the equipment is added.

.. image:: images/move-equipment_4.PNG
    :align: center