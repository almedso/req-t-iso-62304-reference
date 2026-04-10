Hazards
=======

Hazards Probabilities
---------------------

.. list-table:: Hazards Probabilities
   :header-rows: 1

   * - Probability
     - Description
     - Value
   * - Very Low
     - Unlikely to occur under normal operating conditions.
     - x < 0.0001
   * - Low
     - Somewhat unlikely to occur under normal operating conditions.
     - 0.0001 > x > 0.00001
   * - Medium
     - Possible under normal operating conditions.
     - 0.0001 > x > 0.001
   * - High
     - Likely to occur under normal operating conditions.
     - 0.001 > x > 0.01
   * - Very High
     - Almost certain to occur under normal operating conditions.
     - x > 0.1


Hazardous Situations
--------------------

.. hazard:: Misinterpretation of device status
   :id: HAZ_001
   :probability: Medium
   :causes: RSK_001

   The user misinterprets the displayed system status.


.. hazard:: Failure to display status
   :id: HAZ_002
   :probability: Low
   :causes: RSK_002

    The system fails to display the operational status information.