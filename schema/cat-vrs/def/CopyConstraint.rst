
.. note:: This data class is at a **trial use** maturity level and may change
    in future releases. Maturity levels are described in the :ref:`maturity-model`.
                      
                    
**Computational Definition**

The quantity of copies or the type of copy change that a member of this categorical variant must have. One and only one MUST be specified.

**Information Model**

Some CopyConstraint attributes are inherited from :ref:`Constraint`.

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
      - MUST be "CopyConstraint"
   *  - copies
      - integer | :ref:`Range`
      - 0..1
      - The precise value or range of copies a member of this categorical variant must have.
   *  - copyChange
      - string
      - 0..1
      - The type of copy change a member of this categorical variant must have.
