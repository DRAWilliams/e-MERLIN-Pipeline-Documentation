Quick Start
==========+

.. _quickstart:

Quick start
------------

If you have received calibrated data from the observatory and you want to refine the calibration, you can:

.. code-block:: console

   (.venv) $ casa -c eMERLIN_CASA_pipeline/eMERLIN_CASA_pipeline.py -r calibration

#Creating recipes
#----------------

#To retrieve a list of random ingredients,
#you can use the ``lumache.get_random_ingredients()`` function:

#.. autofunction:: lumache.get_random_ingredients
#
#The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
#or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
#will raise an exception.
#
#.. autoexception:: lumache.InvalidKindError
#
#For example:
#
#>>> import lumache
#>>> lumache.get_random_ingredients()
#['shells', 'gorgonzola', 'parsley']

