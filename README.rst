
Installing
============

.. code-block:: bash

    pip install data-conversion-tff==1.0

Usage
=====

.. code-block:: bash

    from data_conversion_tff import main
    main.Reader(data_type,dataset)
   
  .. code-block:: bash
    
    Reader function:
     data_type = 'csv'
     input_path = '/content/drive/MyDrive/Divya-Yasaman/v2/data/csv/chipotle_stores.csv'
     
     or
     
     data_type = 'text'
     input_path = '/content/drive/MyDrive/Vesal-Yasaman/v2/data/text/topics_sample'  # accepts either folder or csv file


     data_type = 'image'
     input_path = '/content/drive/MyDrive/Divya-Yasaman/v2/data/image/fish_sample'  # accepts folder only
