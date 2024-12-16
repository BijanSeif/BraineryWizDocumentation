.. _plotmodelretconspy:

show_constrained and not_show_retained_list and constrained_size Options
========================================================================
Setting show_constrained equal True will cause to plot the retained and constrained nodes connected to each other. constrained_size enable users to determine the size of lines and costrained and retained nodes. By defining list of retained nodes tag and assign to not_show_retained_list, the nodes that their tags are mentioned in the list and nodes that are constrained to them won't be shown using show_constrained. (Default: show_constrained=True,  not_show_retained_list=[], constrained_size=6)

Users also can use **RGquivers_size** option that accepts an float the is size of an arrow that shows a path from constrained node to retained node. This is useful for zerolength element when combine it with :ref:`Shrink_size <plotmodelshrink>` as shown in the second following plot that shows the path of constrained nodes to retained node/s. Also, for plotting nodes that are constrained to another node is useful (first plot).

Example
--------

.. code-block:: python
   :caption: Example for show_constrained=True, constrained_size=6
   
   import BraineryWiz as bz
   
   # ...
   # Create the OpenSees model
   # ...
   
   # Call PlotModel command 
   bz.PlotModel(plotmode=1, show_constrained=True, constrained_size=6, RGquivers_size=5)
   
.. raw:: html
       :file: files/retained.html
	   
.. raw:: html
       :file: files/retained2.html