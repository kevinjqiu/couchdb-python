CouchDB-Python Library
======================

.. image:: https://travis-ci.org/djc/couchdb-python.svg
    :target: https://travis-ci.org/djc/couchdb-python

A Python library for working with CouchDB. `Downloads`_ are available via `PyPI`_.
Our `documentation`_ is also hosted there. We have a `mailing list`_.

This package currently encompasses four primary modules:

* ``couchdb.client``: the basic client library
* ``couchdb.design``: management of design documents
* ``couchdb.mapping``: a higher-level API for mapping between CouchDB documents and Python objects
* ``couchdb.view``: a CouchDB view server that allows writing view functions in Python

It also provides a couple of command-line tools:

* ``couchdb-dump``: writes a snapshot of a CouchDB database (including documents, attachments, and design documents) to MIME multipart file
* ``couchdb-load``: reads a MIME multipart file as generated by couchdb-dump and loads all the documents, attachments, and design documents into a CouchDB database
* ``couchdb-replicate``: can be used as an update-notification script to trigger replication between databases when data is changed

Prerequisites:

* simplejson (or Python >= 2.6, which comes with a simplejson-based JSON module in the standard library)
* Python 2.6 or later
* CouchDB 0.10.x or later (0.9.x should probably work, as well)

.. _Downloads: http://pypi.python.org/pypi/CouchDB
.. _PyPI: http://pypi.python.org/
.. _documentation: http://packages.python.org/CouchDB/
.. _mailing list: http://groups.google.com/group/couchdb-python
