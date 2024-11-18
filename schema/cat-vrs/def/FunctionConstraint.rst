.. note:: This data class is at a **draft** maturity level and may \
    change in future releases. Maturity \
    levels are described in the :ref:`maturity-model`.

**Computational Definition**

A categorical label of the function change that members of this categorical variant satisfies.

**Information Model**

Some FunctionConstraint attributes are inherited from :ref:`Constraint`.

.. list-table::
    :class: clean-wrap
    :header-rows: 1
    :align: left
    :widths: auto

   *  - Field
      - Flags
      - Type
      - Limits
      - Description
   *  - type
      -
      - string
      - 1..1
      - MUST be "FunctionConstraint"
   *  - functionConsequence
      -
      - string
      - 1..1
      - A categorical label of the function change that members of this categorical variant satisfies, using ontology terms from [The Sequence Ontology](http://www.sequenceontology.org).
