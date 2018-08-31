.. _Status-Bar:

Status Bar
----------

The bottom left of the Status Bar will indicate the state of THRUX.  It will change colors as the state changes.

.. image: images/status_bar_1.PNG
    :align: center

.. image: images/status_bar_2.PNG
    :align: center

The bottom right of the Status Bar provides a few more Utility functions to the designer.

The Toggle Flags (Red Flag) button will toggle the visibility settings of all Flags.  

#################
Design Assistance
#################

Different Design Mode Levels are togglable in THRUX, which are indicated by the three lightning symbols.  The default mode is Full Design Assistance, which references the applicable safety codes, standards, and user settings to calculate code minimum values.

*******************************************************************************************************************************************************************************************************************************************************************************************

Full Design Assistance
+++++++++++++++++++++++

Any change in circuit properties will trigger a recalculation in all relevant code minimum values.

.. image:: images/status_bar_utility_1.PNG
    :align: center

Limited Design Assistance
+++++++++++++++++++++++++

Any change in circuit properties will trigger a recalculation in all relevant code minimum values which are not omitted by the Auto-Sizing Settings.  Flags will still be raised as long as they are enabled.

.. image:: images/status_bar_utility_2.PNG
    :align: center

No Design Assistance
++++++++++++++++++++

Designer has full manual control of all circuit properties.  No auto-sizing will be performed.

.. image:: images/status_bar_utility_3.PNG
    :align: center

*******************************************************************************************************************************************************************************************************************************************************************************************

Force Calculation Refresh
+++++++++++++++++++++++++
Refreshes all calculations on the active workspace.

Version
+++++++
Tracks the current Version of THRUX.