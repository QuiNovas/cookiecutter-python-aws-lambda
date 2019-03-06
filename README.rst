==============================
cookiecutter-python-aws-lambda
==============================

.. _Cookiecutter: http://cookiecutter.readthedocs.org
.. _how to create a lambda python deployment package: https://docs.aws.amazon.com/lambda/latest/dg/lambda-python-how-to-create-deployment-package.html

This is a `Cookiecutter`_ template for creating a Python AWS Lambda project.

This project is based loosely on the guidelines specified in
`how to create a lambda python deployment package`_.

Template Project Features
-------------------------

.. _APL2 License: https://choosealicense.com/licenses/apache-2.0/
.. _lambda-setuptools: https://github.com/QuiNovas/lambda-setuptools
.. _CircleCI: https://circleci.com/
.. _Bitbucket Pipelines: https://bitbucket.org/product/features/pipelines

- Python 2.7, 3.4+
- `APL2 License`_
- `lambda-setuptools`_
- `CircleCI`_
- `Bitbucket Pipelines`_

Template Application Features
-----------------------------

- Construction of a ZIP deployment package for your function
- Build scripts for `CircleCI`_ and `Bitbucket Pipelines`_
- Upload of the package to the AWS S3 bucket of choose
- Automatic inclusion of `APL2 License`_, or any license you specify

Usage
-----

.. _GitHub: https://github.com/QuiNovas/cookiecutter-python-aws-lambda


Install Python requirements for using the template:

.. code-block:: console

    $ python -m pip install --requirement=requirements.txt --user


Create a new project directly from the template on `GitHub`_:

.. code-block:: console

    $ cookiecutter gh:QuiNovas/cookiecutter-python-aws-lambda

Items
-----
- **author_email** The email of the author (you) to embed in the Python package
- **author_name** The name of the author (you)
- **circleci_lupload_context** The `CircleCI`_ context containing the required environment variables for upload. See the `CircleCI`_ config file for details
- **dev_status** The development status to embed in the Python package
- **lambda_description** The short description for your Lambda function
- **lambda_name** The name of your Lambda function - also is used as the project's directory name
- **lambda_python_version** The Python version that your function expects
- **lambda_version** The version of your Lambda function
- **license** The license of your Lambda function
- **long_description** The long description of your lambda function
- **lupload_prefix** The AWS S3 object prefix to use on package upload
