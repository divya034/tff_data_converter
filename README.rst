
Installing
============

.. code-block:: bash

    pip install data-conversion-tff==1.0

Usage
=====

.. code-block:: bash

    from data_conversion_tff import main
    main.Reader(data_type, dataset)
   
Functions
=====

1. Reader function: 
Create an object of class reader to access its member functions
      Arguments:
      a. data_type: 'csv' or 'text' or 'image' 
      b. dataset: link your dataset i.e input_path
      
Example: 
Object = main.Reader(data_type, dataset)


2. read_data():
Member function of the Class reader to extract the data and its labels.
        Arguments:
        None
Example:
data, labels = obj.read_data()
   
   Note: For CSV dataset, last csv column is considered as the label.
   
