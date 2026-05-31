
.. |nbsp| unicode:: 0xA0
   :ltrim:
   :rtrim:

.. raw:: latex

    \pagestyle{plain}
    \thispagestyle{plain}
    \osiaskipnextchapter
    %% Suppress all TOC entries for the overview chapter (sections, subsections,
    %% Copyright addcontentsline) — restored just before \sphinxtableofcontents
    %% so chapters from Introduction onward appear in the TOC normally.
    \let\osiaorigaddcontentsline\addcontentsline
    \renewcommand{\addcontentsline}[3]{}

.. _chapter-overview:

Overview
========

.. raw:: latex

    \osiacenternextsection

ITU-T X-Series Recommendations
------------------------------

.. list-table:: Data networks, open system communications and security
    :header-rows: 0
    :widths: 72 28
    :class: itu-xseries

    * - PUBLIC DATA NETWORKS
      - X.1–X.199
    * - OPEN SYSTEMS INTERCONNECTION
      - X.200–X.299
    * - INTERWORKING BETWEEN NETWORKS
      - X.300–X.399
    * - MESSAGE HANDLING SYSTEMS
      - X.400–X.499
    * - DIRECTORY
      - X.500–X.599
    * - OSI NETWORKING AND SYSTEM ASPECTS
      - X.600–X.699
    * - OSI MANAGEMENT
      - X.700–X.799
    * - SECURITY
      - X.800–X.849
    * - OSI APPLICATIONS
      - X.850–X.899
    * - OPEN DISTRIBUTED PROCESSING
      - X.900–X.999
    * - INFORMATION AND NETWORK SECURITY
      - X.1000–X.1099
    * - SECURE APPLICATIONS AND SERVICES (I)
      - X.1100–X.1199
    * - CYBERSPACE SECURITY
      - X.1200–X.1299
    * - |nbsp| |nbsp| |nbsp| |nbsp| Cybersecurity
      - |nbsp| |nbsp| |nbsp| |nbsp| X.1200–X.1229
    * - |nbsp| |nbsp| |nbsp| |nbsp| Countering spam
      - |nbsp| |nbsp| |nbsp| |nbsp| X.1230–X.1249
    * - |nbsp| |nbsp| |nbsp| |nbsp| **Identity management (IdM) and Authentication**
      - |nbsp| |nbsp| |nbsp| |nbsp| **X.1250–X.1299**
    * - SECURE APPLICATIONS AND SERVICES (II)
      - X.1300–X.1499
    * - CYBERSECURITY INFORMATION EXCHANGE
      - X.1500–X.1599
    * - CLOUD COMPUTING SECURITY
      - X.1600–X.1699
    * - QUANTUM COMMUNICATION
      - X.1700–X.1729
    * - DATA SECURITY
      - X.1750–X.1799
    * - INTERNATIONAL MOBILE TELECOMMUNICATIONS (IMT) SECURITY
      - X.1800–X.1839
    * - METAVERSE AND DIGITAL TWIN SECURITY
      - X.2000–X.2199
    * - SOFTWARE SUPPLY CHAIN SECURITY
      - X.2150–X.2199
    * - ARTIFICIAL INTELLIGENCE (AI) / MACHINE LEARNING (ML) SECURITY
      - X.2200–X.2249

*For further details, please refer to the list of ITU-T Recommendations.*

.. raw:: latex

    \newpage

Recommendation ITU-T X.1281
---------------------------

.. only:: html

    **APIs for interoperability of identity management systems**

.. raw:: latex

    \begin{center}\textbf{APIs for interoperability of identity management systems}\end{center}

Summary
"""""""

Recommendation ITU-T X.1281 describes a set of standardized application program
interfaces (APIs) needed to connect the multiple building blocks of an identity
management solution.

.. note::

    This Recommendation is technically equivalent to the OSIA specification (see [b-OSIA]
    in the bibliography).

History
"""""""

.. list-table::
    :header-rows: 1
    :widths: 10 26 18 14 32

    * - Edition
      - Recommendation
      - Approval
      - Study Group
      - Unique ID
    * - 1.0
      - ITU-T X.1281
      - 2024-03-01
      - 17
      - 11.1002/1000/15662

To access the Recommendation, type the URL https://handle.itu.int/ in the address field
of your web browser, followed by the Recommendation's unique ID.

Keywords
""""""""

Authentication, identity management, interoperability.

.. raw:: latex

    \newpage
    \osiacenternextsubsection

Foreword
""""""""

The International Telecommunication Union (ITU) is the United Nations specialized agency
in the field of telecommunications, information and communication technologies (ICTs).
The ITU Telecommunication Standardization Sector (ITU-T) is a permanent organ of ITU.
ITU-T is responsible for studying technical, operating and tariff questions and issuing
Recommendations on them with a view to standardizing telecommunications on a worldwide basis.

The World Telecommunication Standardization Assembly (WTSA), which meets every four years,
establishes the topics for study by the ITU-T study groups which, in turn, produce
Recommendations on these topics.

The approval of ITU-T Recommendations is covered by the procedure laid down in WTSA Resolution 1.

In some areas of information technology which fall within ITU-T's purview, the necessary
standards are prepared on a collaborative basis with ISO and IEC.

.. raw:: latex

    \osiacenternextsubsection

Note
""""

In this Recommendation, the expression "Administration" is used for conciseness to indicate
both a telecommunication administration and a recognized operating agency.

Compliance with this Recommendation is voluntary. However, the Recommendation may contain
certain mandatory provisions (to ensure, e.g., interoperability or applicability) and
compliance with the Recommendation is achieved when all of these mandatory provisions are met.
The words "shall" or some other obligatory language such as "must" and the negative
equivalents are used to express requirements. The use of such words does not suggest that
compliance with the Recommendation is required of any party.

.. raw:: latex

    \osiacenternextsubsection

Intellectual Property Rights
""""""""""""""""""""""""""""

ITU draws attention to the possibility that the practice or implementation of this
Recommendation may involve the use of a claimed Intellectual Property Right. ITU takes no
position concerning the evidence, validity or applicability of claimed Intellectual Property
Rights, whether asserted by ITU members or others outside of the Recommendation development
process.

As of the date of approval of this Recommendation, ITU had not received notice of intellectual
property, protected by patents/software copyrights, which may be required to implement this
Recommendation. However, implementers are cautioned that this may not represent the latest
information and are therefore strongly urged to consult the appropriate ITU-T databases
available via the ITU-T website at http://www.itu.int/ITU-T/ipr/.
Implementers should also be aware that the organization that originated the technically
equivalent document listed in the Bibliography may have received notices of intellectual
property required for the implementation of this Recommendation.

.. raw:: latex

    \vspace{4em}
    \begin{center}\textcopyright{} ITU 2024\end{center}

    \medskip
    All rights reserved. No part of this publication may be reproduced, by any means whatsoever, without the
    prior written permission of ITU.

    %% Restore \addcontentsline so the TOC below (and Chapter 1 onward) populate.
    \let\addcontentsline\osiaorigaddcontentsline
    \sphinxtableofcontents
    \osiamainmatter
