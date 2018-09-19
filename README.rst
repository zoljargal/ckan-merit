.. You should enable this project on travis-ci.org and coveralls.io to make
   these badges work. The necessary Travis and Coverage config files have been
   generated for you.

.. image:: https://travis-ci.org/zoljargal/ckanext-merit.svg?branch=master
    :target: https://travis-ci.org/zoljargal/ckanext-merit

.. image:: https://coveralls.io/repos/zoljargal/ckanext-merit/badge.svg
  :target: https://coveralls.io/r/zoljargal/ckanext-merit

.. image:: https://pypip.in/download/ckanext-merit/badge.svg
    :target: https://pypi.python.org/pypi//ckanext-merit/
    :alt: Downloads

.. image:: https://pypip.in/version/ckanext-merit/badge.svg
    :target: https://pypi.python.org/pypi/ckanext-merit/
    :alt: Latest Version

.. image:: https://pypip.in/py_versions/ckanext-merit/badge.svg
    :target: https://pypi.python.org/pypi/ckanext-merit/
    :alt: Supported Python versions

.. image:: https://pypip.in/status/ckanext-merit/badge.svg
    :target: https://pypi.python.org/pypi/ckanext-merit/
    :alt: Development Status

.. image:: https://pypip.in/license/ckanext-merit/badge.svg
    :target: https://pypi.python.org/pypi/ckanext-merit/
    :alt: License

=============
ckanext-merit
=============

.. Put a description of your extension here:
   What does it do? What features does it have?
   Consider including some screenshots or embedding a video!


------------
Requirements
------------

For example, you might want to mention here which versions of CKAN this
extension works with.


------------
Installation
------------

.. Add any additional install steps to the list below.
   For example installing any non-Python dependencies or adding any required
   config settings.

To install ckanext-merit:

1. Activate your CKAN virtual environment, for example::

     . /usr/lib/ckan/default/bin/activate

2. Install the ckanext-merit Python package into your virtual environment::

     pip install ckanext-merit

3. Add ``merit`` to the ``ckan.plugins`` setting in your CKAN
   config file (by default the config file is located at
   ``/etc/ckan/default/production.ini``).

4. Restart CKAN. For example if you've deployed CKAN with Apache on Ubuntu::

     sudo service apache2 reload


---------------
Config Settings
---------------

Document any optional config settings here. For example::

    # The minimum number of hours to wait before re-checking a resource
    # (optional, default: 24).
    ckanext.merit.some_setting = some_default_value


------------------------
Development Installation
------------------------

To install ckanext-merit for development, activate your CKAN virtualenv and
do::

    git clone https://github.com/zoljargal/ckanext-merit.git
    cd ckanext-merit
    python setup.py develop
    pip install -r dev-requirements.txt


-----------------
Running the Tests
-----------------

To run the tests, do::

    nosetests --nologcapture --with-pylons=test.ini

To run the tests and produce a coverage report, first make sure you have
coverage installed in your virtualenv (``pip install coverage``) then run::

    nosetests --nologcapture --with-pylons=test.ini --with-coverage --cover-package=ckanext.merit --cover-inclusive --cover-erase --cover-tests


---------------------------------
Registering ckanext-merit on PyPI
---------------------------------

ckanext-merit should be availabe on PyPI as
https://pypi.python.org/pypi/ckanext-merit. If that link doesn't work, then
you can register the project on PyPI for the first time by following these
steps:

1. Create a source distribution of the project::

     python setup.py sdist

2. Register the project::

     python setup.py register

3. Upload the source distribution to PyPI::

     python setup.py sdist upload

4. Tag the first release of the project on GitHub with the version number from
   the ``setup.py`` file. For example if the version number in ``setup.py`` is
   0.0.1 then do::

       git tag 0.0.1
       git push --tags


----------------------------------------
Releasing a New Version of ckanext-merit
----------------------------------------

ckanext-merit is availabe on PyPI as https://pypi.python.org/pypi/ckanext-merit.
To publish a new version to PyPI follow these steps:

1. Update the version number in the ``setup.py`` file.
   See `PEP 440 <http://legacy.python.org/dev/peps/pep-0440/#public-version-identifiers>`_
   for how to choose version numbers.

2. Create a source distribution of the new version::

     python setup.py sdist

3. Upload the source distribution to PyPI::

     python setup.py sdist upload

4. Tag the new release of the project on GitHub with the version number from
   the ``setup.py`` file. For example if the version number in ``setup.py`` is
   0.0.2 then do::

       git tag 0.0.2
       git push --tags
