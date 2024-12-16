.. _plotmodelshrink:

Shrink_Size Option
====================================================
A float value less than 1 that shrinks elements according the value that has been assigned to this feature or option. Mainly this feature helps users to understand their zerolength elements modeling. As shown in the following plot, it can be seen that elements of plot has been shrinked and zerolength elements now has length and show their both head nodes. (Attention that in this plot show_nodes_tag option has been turned on)

Example
--------

.. code-block:: python
   :caption: Example for Shrink_Size=0.7
   
   import BraineryWiz as bz
   
   # ...
   # Create the OpenSees model
   # ...
   
   # Call PlotModel command 
   bz.PlotModel(plotmode=1, Shrink_Size=0.7)

.. raw:: html
       :file: files/shrink.html
	   