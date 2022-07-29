
Installing
============

.. code-block:: bash

    pip install data-conversion-tff==1.0

Usage
=====

.. code-block:: bash

    from data_conversion_tff import main
    obj = main.Reader(data_type, dataset)
    
    data, labels = obj.read_data()

    NUM_CLIENTS = 10
    SELECTED_FEATURE = 1
    dataset = main.convert_to_client_data(data, labels,  data_type,
                                                dist_type = 'niid',
                                                number_of_clients = NUM_CLIENTS,
                                                selected_feature=SELECTED_FEATURE,
                                                min_seen_labels=2,
                                                max_seen_labels=3
                                                )
   
Functions (not completed)
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
   
