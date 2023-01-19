Creating an Object Storage Bucket
=================================

Exercise 4: Create an Object Storage Bucket
-------------------------------------------
Objectives

#. Build an Object Storage Bucket
#. Connect to the Object Storage Bucket with Cyberduck
#. Connect to the Object Storage Bucket with AWS Command Line Interface

Configuration

*	**Name:** my-bucket-NAME or INITIAL – e.g., my-bucket-JohnSmith, my-bucket-JS

Connect to the Object Storage Bucket with AWS Command Line Interface (CLI)

.. code-block:: console

   $ aws configure
   
.. code-block:: console

   AWS Access Key ID [None]: <AWS Access Key ID>
   AWS Secret Access Key [None]: <AWS Secret Access Key>
   Default region name [None]: ca-central-1
   Default output format [None]: JSON

.. code-block:: console

   $ aws s3 ls my-bucket-mt.store.ubc-hpc.cloud

.. code-block:: console

   2023-01-06 18:04:31        11  test.txt

Links

* **Instructions:** https://blog.ronin.cloud/object-storage/
* **Connect via Cyberduck:** https://blog.ronin.cloud/windows-mac-object-storage/
*	**Connect via AWS CLI:** https://blog.ronin.cloud/linux-object-storage/ 
* **Cyberduck:** https://cyberduck.io/ 
