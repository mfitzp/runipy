``runipynb``: run IPython as a script
===================================

The IPython notebook provides an interactive interface to a Python interpreter.

- **Literate programming**: the IPython notebook is an ideal format for
  writing "literate" programs, in which the code is part of a larger multi-media
  document. ``runipynb`` lets you run such programs directly, without first
  converting to a pure Python script.
- **Report generation**: ``runipynb`` can run the notebook and convert it into HTML
  in one go, making it an easy way to automate reports when aesthetic control
  is not a priority.
- **Data pipeline**: if you use IPython notebooks to create a data pipeline,
  ``runipynb`` lets you automate that pipeline without loosing the notebook
  formatting.

Installation
------------

The easiest way to install ``runipy`` is with ``pip``::

    $ pip install runipy

Use
---

To run a ``.ipynb`` file as a script, run::

    $ runipynb MyNotebook.ipynb

To save the output of each cell back to the notebook file, run::

    $ runipynb -o MyNotebook.ipynb

To save the notebook output as a *new* notebook, run::

    $ runipynb MyNotebook.ipynb OutputNotebook.ipynb

To run a ``.ipynb`` file and genereate an ``HTML`` report, run::

    $ runipynb MyNotebook.ipynb --report report.html

