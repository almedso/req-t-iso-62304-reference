Risk Management Traceability Matrix
===================================

Hassards and Risks
-------------------

.. needtable::
   :style: table
   :filter: type == "hassard" and causes
   :update: severity = causes|map(attribute='severity')|max
   :columns: id, title, probability, triggers, severity

Risk Controls Coverage
-----------------------

.. needtable::
   :style: table
   :filter: len(mitigates) > 0
   :columns: id, title, mitigates

Unmitigated Risks
-----------------------

.. needtable::
   :style: table
   :filter: type == "risk" and not mitigates_back
   :columns: id, title