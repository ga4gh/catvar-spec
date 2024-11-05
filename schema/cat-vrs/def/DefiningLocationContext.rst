
.. warning:: This data class is at a **draft** maturity level and may change
    significantly in future releases. Maturity levels are described in 
    the :ref:`maturity-model`.
                      
                    
**Computational Definition**

The defining location and its associated relationships that are congruent with member locations.

**Information Model**

Some DefiningLocationContext attributes are inherited from :ref:`Constraint`.

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
      - MUST be "DefiningLocationContext"
   *  - location
      - :ref:`SequenceLocation` | :ref:`IRI`
      - 1..1
      - 
   *  - relations
      - string
      - 0..m
      - Defined relationships from which members relate to the defining context. ``sequence_liftover`` refers to variants or locations that represent a congruent concept on a differing assembly of a human genome (e.g. "GRCh37" and "GRCh38") or gene (e.g. Locus Reference Genomic) sequence. ``transcript_projection`` refers to variants or locations that occur on transcripts projected from the defined genomic concept. ``codon_translation`` refers to variants or locations that translate from the codon(s) represented by the defined concept.
   *  - matchCharacteristic
      - string
      - 1..1
      - A characteristic of the location that is used to match the defining location to member locations. 
