
Section title
-------------

.. admonition:: Note title

    Lorem ipsum dolor sit amet, consectetur adipiscing elit:

    - Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua
    - Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
    - Nisi ut aliquip ex ea commodo consequat


Subsection title
""""""""""""""""

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
laboris nisi ut aliquip ex ea commodo consequat.

Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat
nulla pariatur.

Subsection title
""""""""""""""""

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua.


Subsection title
""""""""""""""""

.. uml::
    :caption: Example Data Model
    :scale: 50%

    class EntityA {
        string identifier;
    }

    class EntityB {
        string field1;
        date field2;
        ...
    }
    EntityA o- EntityB

    class EntityC {
        string field1;
        int field2;
        date field3;
        ...
    }
    EntityC -o EntityA

    class EntityD {
        byte[] data;
        URL reference;
    }
    EntityA o-- "*" EntityD
