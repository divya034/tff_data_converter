
Installing
============

.. code-block:: bash

    pip install data-conversion-tff==1.0

Usage
=====

.. code-block:: bash

    from data_conversion_tff import main


     data_type = 'image' # type image or csv
     
     input_path = r'C:\Users\beaut\OneDrive\Desktop\mitacs\fish_sample_3' #insert the link
     
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
   

