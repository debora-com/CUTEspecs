
.. _chapter2:

Chapter title
=============
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
laboris nisi ut aliquip ex ea commodo consequat.

Section title
-------------

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. The building blocks are defined as follows:

- The *Building Block One*.

  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
  incididunt ut labore et dolore magna aliqua.

- The *Building Block Two*.

  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
  incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
  exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. [#]_

- The *Building Block Three*.

  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
  incididunt ut labore et dolore magna aliqua.

.. note::

   Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
   incididunt ut labore et dolore magna aliqua.

Lorem ipsum dolor sit amet:

.. figure:: images/components.png
    :width: 90%

    Lorem ipsum dolor sit amet

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua.

.. py:function:: subscribe(topic,URL)
    :noindex:

    Subscribe a URL to receive notifications sent to one topic

    **Authorization**: ``notif.sub.write``

    :param str topic: Topic
    :param str URL: URL to be called when a notification is available
    :return: a subscription ID

This service is synchronous.

Section title
-------------

Lorem ipsum dolor sit amet:

- Interface One

  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.

- Interface Two

  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.
  
    ``application[.resource].action``

- Interface Three

  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.

The following table describes in detail the interfaces and associated services.

.. table:: Interfaces List
    :class: longtable
    :widths: 30 70

    ================================= ===================================================================================
    **Services**                       **Description**
    ================================= ===================================================================================
    **Group One**
    ---------------------------------------------------------------------------------------------------------------------
    Service One                        Lorem ipsum dolor sit amet, consectetur adipiscing elit
    Service Two                        Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua
    Service Three                      Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
    Service Four                       Nisi ut aliquip ex ea commodo consequat
    Service Five                       Duis aute irure dolor in reprehenderit in voluptate velit
    --------------------------------- -----------------------------------------------------------------------------------
    **Group Two**
    ---------------------------------------------------------------------------------------------------------------------
    Service Six                        Esse cillum dolore eu fugiat nulla pariatur
    Service Seven                      Excepteur sint occaecat cupidatat non proident
    Service Eight                      Sunt in culpa qui officia deserunt mollit anim id est laborum
    Service Nine                       Sed ut perspiciatis unde omnis iste natus error sit voluptatem
    Service Ten                        Accusantium doloremque laudantium totam rem aperiam
    ================================= ===================================================================================


Section title
-------------

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua.

Considering the following JSON, describing an identity with one biometric and one supporting document:

.. code-block:: json

    {
        "identityType": "string",
        "status": "CLAIMED",
        "galleries": ["SAMPLE"],
        "clientData": "c3RyaW5n",
        "contextualData": {
        },
        "biographicData": {
            "lastName": "Smith",
            "firstName": "Alice",
            "dateOfBirth": "1987-11-30",
            "gender": "F",
            "nationality": "FRA"
        },
        "biometricData": [
            {
                "biometricType": "FINGER",
                "biometricSubType": "RIGHT_INDEX",
                "image": "SU1BR0UgQlVGRkVSIEJBU0U2NCBFTkNPREVE",
                "vendor": "SIA"
            }
        ],
        "documentData": [
            {
                "documentType": "FORM",
                "parts": [
                    {
                        "pages": [
                            1,
                            2
                        ],
                        "data": "c3RyaW5n",
                        "mimeType": "application/pdf",
                        "captureDate": "2019-05-21T12:00:00+02:00"
                    },
                    {
                        "pages": [
                            3
                        ],
                        "data": "c3RyaW5n",
                        "mimeType": "application/pdf",
                        "captureDate": "2019-05-21T12:00:00+02:00"
                    }
                ]
            }
        ]
    }


.. warning::

    Bearer tokens are sensitive and subject to security issues if not handled properly. Please refer to
    :rfc:`8725` for *JSON Web Token Best Current Practices* and advice on proper implementation.

Subsection title
""""""""""""""""

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
laboris nisi ut aliquip ex ea commodo consequat.

.. uml::
    :caption: Example Use Case
    :scale: 50%

    hide footbox
    actor "Actor" as actor
    participant "Service A" as A
    participant "Service B" as B
    participant "Service C" as C

    actor -> A
    activate actor
    activate A

    group 1. Step One
        A -> B: serviceCall(parameters)
        A -> B: serviceCall(parameters)
        A -> B: readData(parameters)
        A -> A: Additional processing
    end

    group 2. Step Two
        A -> C: generateResult()
        A -> A
        note right: perform the operation

        A -->> actor: result
        destroy actor
    end

    group 3. Step Three
        A -->> B: event(data)
        deactivate A

        ...

        B -> A: readData(parameters)
        activate B
        B -> A: readData(parameters)
        B -> B
        note right
          process the event
          update records
        end note
        deactivate B
    end

1. Step One

   Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt:

   - ``serviceCall``: lorem ipsum dolor sit amet, consectetur adipiscing elit
   - ``readData``: sed do eiusmod tempor incididunt ut labore et dolore magna aliqua
   - ``generateResult``: ut enim ad minim veniam, quis nostrud exercitation ullamco laboris

   Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat
   nulla pariatur.

2. Step Two

   Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt
   ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
   laboris nisi ut aliquip ex ea commodo consequat.


.. rubric:: Footnotes

.. [#] *Handbook on Civil Registration and Vital Statistics Systems: Management, Operation and Maintenance,
   Revision 1, United Nations, New York, 2018, available at:*
   https://unstats.un.org/unsd/demographic-social/Standards-and-Methods/files/Handbooks/crvs/crvs-mgt-E.pdf *, para 65.*

.. [#] *Principles and Recommendations for a Vital Statistics System, United Nations publication
   Sales Number E.13.XVII.10, New York, 2014, paragraph 279*
