.. _launch_all_conversion_nodes:

Launch all Conversion Nodes
###########################

A launch file that starts all nodes that convert vision data to
marker / marker-arrays for visualization in RViz.

In a terminal, run:

.. code-block:: console

  ros2 launch soccer_marker_generation all.launch.py

Subscription Topics
*******************

* `vision/ball` (`soccer_object_msgs/msg/Ball`_)
* `vision/goalposts` (`soccer_object_msgs/msg/GoalpostArray`_)
* `vision/field_lines` (`soccer_object_msgs/msg/FieldLineArray`_)
* `vision/flags` (`soccer_object_msgs/msg/FlagArray`_)
* `vision/robots` (`soccer_object_msgs/msg/RobotArray`_)

Publishing Topics
*****************

* `visualization/ball` (`visualization_msgs/Marker`_)
* `visualization/goalposts` (`visualization_msgs/MarkerArray`_)
* `visualization/field_lines` (`visualization_msgs/MarkerArray`_)
* `visualization/flags` (`visualization_msgs/MarkerArray`_)
* `visualization/robots` (`visualization_msgs/MarkerArray`_)


.. tip::

  It is recommended to create your own launch file, similar to ``all.launch.py`` that launches only the nodes you need.


.. _soccer_object_msgs/msg/Ball: https://soccer-object-msgs.readthedocs.io/en/latest/vision_msgs.html#ball
.. _soccer_object_msgs/msg/GoalpostArray: https://soccer-object-msgs.readthedocs.io/en/latest/vision_msgs.html#goalpostarray
.. _soccer_object_msgs/msg/FieldLineArray: https://soccer-object-msgs.readthedocs.io/en/latest/vision_msgs.html#fieldlinearray
.. _soccer_object_msgs/msg/FlagArray: https://soccer-object-msgs.readthedocs.io/en/latest/vision_msgs.html#flagarray
.. _soccer_object_msgs/msg/RobotArray: https://soccer-object-msgs.readthedocs.io/en/latest/vision_msgs.html#robotarray
.. _visualization_msgs/Marker: http://docs.ros.org/en/api/visualization_msgs/html/msg/Marker.html
.. _visualization_msgs/MarkerArray: http://docs.ros.org/en/noetic/api/visualization_msgs/html/msg/MarkerArray.html