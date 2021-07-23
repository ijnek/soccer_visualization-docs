Installation
############

.. note::

    Instructions here assume that you have and are in the ROS2 workspace
    root directory.

Cloning repositories
********************

In your ROS2 workspace, clone the repository:

.. code-block:: console

   git clone https://github.com/ijnek/soccer_visualization.git src/soccer_visualization
   vcs import src < src/soccer_visualization/dependencies.repos

Building
********

To build the package and its dependencies, in the workspace root directory, run:

.. code-block:: console

   colcon build