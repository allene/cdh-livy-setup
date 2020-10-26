# Installing & setting up Apache Livy on CDH 6.3 cluster
Original code was copied from https://github.com/GoogleCloudDataproc/initialization-actions/tree/master/livy

This `livy_setup.sh` script
installs [Apache Livy](https://livy.incubator.apache.org/) on a node
within a CDH 6.3 cluster.


1.  To change installed Livy version, export `LIVY_VERSION` environment variable:
    
    Examples:
    To install Livy 0.6.0 version
    ```bash
    export LIVY_VERSION=0.6.0;./livy_setup.sh
    ```
    To install Livy 0.7.0 version
    ```bash
    ./livy_setup.sh
    ```
1.  Once the cluster has been created, Livy is configured to run on port `8998`
    on the master node.

1.  To learn about how to use Livy read the documentation for the
    [Rest API](https://livy.incubator.apache.org/docs/latest/rest-api.html)
1.  To learn about setting up sparkmagic check [this document](https://github.com/jupyter-incubator/sparkmagic)