
.. note:: This data class is at a **trial use** maturity level and may change
    in future releases. Maturity levels are described in the :ref:`maturity-model`.
                      
                    
**Computational Definition**

The exact or range of copies that members of this categorical variant must satisfy.

**Information Model**

Some CopyCountConstraint attributes are inherited from :ref:`Constraint`.

.. list-table::
   :class: clean-wrap
   :header-rows: 1
   :align: left
   :widths: auto

   *  - Field
      - Type
      - Limits
      - Description
   *  - type
      - string
      - 1..1
      - MUST be "CopyCountConstraint"
   *  - copies
      - integer | :ref:`Range`
      - 1..1
      - The precise value or range of copies members of this categorical variant must satisfy.
