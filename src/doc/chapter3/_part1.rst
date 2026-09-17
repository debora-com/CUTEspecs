
Section title
-------------

Lorem ipsum dolor sit amet, consectetur adipiscing elit. The following table maps the
interfaces described in :ref:`chapter3` against the building blocks.

.. This is a "simple table". The column text MUST line up under the "=" / "-" border
   characters, otherwise the build fails with "Malformed table". When editing, keep each
   cell within its column width and align new rows to the borders above.

.. table:: Mapping Building Blocks vs Interfaces
    :class: longtable

    =================================  ============  ============  ============
    **Interfaces**                     Block One     Block Two     Block Three
    =================================  ============  ============  ============
    **Group One**
    ---------------------------------------------------------------------------
    Service One                        U             I
    Service Two                        U             I             U
    ---------------------------------  ------------  ------------  ------------
    **Group Two**
    ---------------------------------------------------------------------------
    Service Three                      I                           U
    Service Four                       I             U             U
    =================================  ============  ============  ============



Subsection title
""""""""""""""""

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.

.. list-table:: Example Dictionary
    :header-rows: 1

    * - Event Type
      - Emitted by Block One
      - Emitted by Block Two

    * - Event One
      - |tick|
      -
    * - Event Two
      - |tick|
      -
    * - Event Three
      -
      - |tick|
    * - Event Four
      - |tick|
      - |tick|
