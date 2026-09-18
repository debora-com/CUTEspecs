
.. _chapter3:

============================
Organising a large document
============================

As a specification grows, you will want to split it across several source files.
Sphinx offers two mechanisms, and it is important to understand the difference.

toctree
-------

A ``toctree`` links to other files as *separate pages*, each with its own entry
in the navigation sidebar. This is how the chapters of this document are joined
together (see ``index.rst``), and how Chapter 4 lists its API interfaces.

Use a ``toctree`` when each piece is substantial enough to deserve its own page.
A folder with an ``index.rst`` plus one file per sub-page — as in
``chapter4/`` — is the usual shape. In this template, **a folder means the
section is split into several pages**; a plain ``.rst`` file is a self-contained
section.

You write it like this, listing each sub-page (without the ``.rst`` extension):

.. code-block:: rst

    .. toctree::

        interface1
        interface2

Each listed file becomes its own page, linked in the navigation sidebar.

include
-------

An ``include`` pastes another file's content directly into the current page, as
if you had typed it there. The result is a single continuous page. Use it to
break one long chapter into smaller source files — for example, so several
authors can edit different parts without touching the same file — while the
reader still sees one seamless chapter.

You write it like this, giving the path to each fragment:

.. code-block:: rst

    .. include:: _part1.rst

    .. include:: _part2.rst

The content of each file is inserted in place, producing one continuous page.
Included fragments are named with a leading underscore (for example
``_part1.rst``) so the build skips them as standalone pages.

.. tip::

    A change to an *included* file does not always trigger a rebuild of the page
    that includes it. If an edit does not appear, rebuild fully — the project
    ``HOWTO`` explains how, and the live-preview helper is already configured to
    do this for you.
