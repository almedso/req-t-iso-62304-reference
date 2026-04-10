Software Architecture
=====================

Software Design
===============

User Interface Design
---------------------

.. swspec:: Display format for status
   :id: SWS_001
   :implements: SWR_001

   Line 1: STATUS (READY, ERROR, RUNNING)
   Line 2: Value

.. swspec:: LCD driver module
   :id: SWS_002
   :implements: SWR_001

   The LCD driver shall implement the communication protocol.
