Quick start
=====

.. _quickstart:

If you have received calibrated data from the observatory and you want to refine the calibration, you can:

.. code-block:: console

   (.venv) $ casa -c eMERLIN_CASA_pipeline/eMERLIN_CASA_pipeline.py -r calibration
   


Additional usage instructions
------------------

For a normal pipeline execution and assuming you have a ``inputs.ini`` file, and you have extracted the pipeline, you can:

.. code-block:: console

   (.venv) $ casa -c /path/to/pipeline/eMERLIN_CASA_pipeline.py 
   
To run the parallelized version using MPI in CASA you can use:

.. code-block:: console

   (.venv) $ mpicasa -n <num_cores> -c eMERLIN_CASA_pipeline/eMERLIN_CASA_pipeline.py
   

Optional arguments
------------------

If you have want to run individual tasks, you can type them in:

.. code-block:: console

   (.venv) $ casa -c eMERLIN_CASA_pipeline/eMERLIN_CASA_pipeline.py -r first_images
   
To exclude tasks use the ``-s`` parameter:

.. code-block:: console

   (.venv) $ casa -c eMERLIN_CASA_pipeline/eMERLIN_CASA_pipeline.py -r calibration -s first_images

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

