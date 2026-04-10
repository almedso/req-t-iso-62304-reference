Mandatory Traceability
======================

Software Requirements Not Verified
----------------------------------

.. needlist::
   :filter: type == "swr" and not verifies_back

.. note ::

    It is expected that the list is empty, otherwise we have software requirements
    that are not verified by any test case, which is a problem for regulatory compliance.


SoftwareRequirements without Parent
------------------------------------

.. needlist::
   :filter: type == "sw" and not derives


.. note ::

    It is expected that the list is empty, there are software requirements that
    are not justified by any system requirement or risk mitigation,
    which can be a problem for regulatory compliance.


Arbitrary Traceability
======================

Software Specifications Not Verified
------------------------------------

.. needlist::
   :filter: type == "sws" and not verifies_back

