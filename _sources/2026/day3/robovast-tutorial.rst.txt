***********************
RoboVAST Tutorial
***********************

.. note::

   This tutorial covers the navigation plugin only. The metamorphic testing and FAIR metadata plugins are not covered here.

.. _RoboVAST repository: https://github.com/cps-test-lab/robovast

Prerequisites
=============

- Docker
- Python 3.12
- Ubuntu 24.04 (recommended; Windows also supported)


Installing RoboVAST
===================

Set up a virtual environment:

.. code-block:: bash

   sudo apt install python3-venv
   python3 -m venv venv
   . venv/bin/activate

Clone the repository:

.. code-block:: bash

   git clone https://github.com/cps-test-lab/robovast.git
   cd robovast

Install RoboVAST and the navigation extension:

.. code-block:: bash

   pip install -e .
   pip install -e src/robovast_nav

Verify the installation and optionally enable shell completion:

.. code-block:: bash

   vast --help

   # enable shell completions
   vast install-completion
   source ~/.bashrc  # or source the appropriate file for your shell

Pull the Docker image:

.. code-block:: bash

   docker pull ghcr.io/cps-test-lab/robovast:latest


Download the Example Files
===========================

Download the example ``.vast`` file, scenario file, and environment/setup files.
The expected folder structure is:

.. code-block:: text

   .
   └── RoboVAST Examples
       ├── analysis/
       ├── environments/
       │   ├── hbrs_c/
       │   ├── hexagon/
       │   ├── hexagon_large/
       │   ├── hexagon_offset/
       │   └── secorolab/
       ├── files/
       ├── examples.vast       # example vast file
       ├── scenario.osc        # example multi-goal scenario file
       └── variations.yaml     # examples of different variation configurations


Running a Validation Campaign
==============================

Initialize the ``.vast`` file
------------------------------

Make sure you are inside the ``RoboVAST Examples`` folder, then run:

.. code-block:: bash

   vast init examples.vast

Launch the configuration GUI
-----------------------------

.. code-block:: bash

   vast config gui

Modify the ``.vast`` file
--------------------------

You only need to change the **configuration section**: modifying, adding, and removing configurations.

- Refer to ``variations.yaml`` for different possible configurations and variation types.
- If you change the maps, keep in mind that the path length and number of goal poses may need to be adjusted so that viable paths can be found (long paths with few goals cannot be generated for small maps; the same applies when many obstacles are present).
- View the generated test cases by pressing the **Generate** button.
- Once finished, save the ``.vast`` file.

Execute the ``.vast`` file locally
------------------------------------

.. code-block:: bash

   vast exec local run


Viewing Results
================

Once the tests have finished running, post-process and visualize the results:

.. code-block:: bash

   vast results postprocess
   vast analysis gui
