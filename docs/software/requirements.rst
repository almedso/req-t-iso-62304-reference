Software Requirements
=====================


User Interface Requirements
-----------------------------

.. swreq:: Software shall provide status information to display
   :id: SWR_001
   :derives: SYR_001

Constraints
===========

.. constraints are a-priori design decisions that limit the solution space
   and guide the implementation of the system.
   They can be derived from technical, economic, regulatory, or other considerations,
   and they can have a significant impact on the design and implementation of the system.


.. con:: Use 2x16 character LCD
   :id: CON_001
   :constrains: SYR_001, SWR_001, SWS_001

   Is a constraint because we have plenty of those displays available,
   and they are cheap.


.. con:: Rust language for embedded control software
   :id: CON_002

   Rust guarantes memory safety, thread safety.
