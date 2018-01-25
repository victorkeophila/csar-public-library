##################
Ystia CSAR library
##################

.. contents::
	:local:
	:depth: 4


.. *********************************************************************************************************************

.. _introduction_section:

************
Introduction
************

Ystia CSAR library overview
===========================

.. **Ystia CSAR libray** provides a packaged solution to create easily Big Data application clusters on demand.
.. Deployment of Big Data applications can be done on a public Cloud (such as Amazon),
.. or on a private cloud (such as OpenStack), on Bare-Metal or on HPC.
..
.. Big Data applications targeted by Ystia are:
..
.. - mainly **Hadoop** applications based on MapR_, Hortonworks_ or Cloudera_.
.. - and **Log Analysis** applications based on Elastic_ components.
..
.. In addition, Ystia CSAR libray provides useful components such as:
..
.. - **SQL** and **Not Only SQL** database servers (MySQL_, MongoDB_, PostgreSQL_),
.. - message brokers (Kafka_),
.. - data science development environments (RStudio_, Jupyter_)
.. - and other technical components such as **Java**, **Consul** (Consensus Systems), allowing detailed application
..   architectures to be designed.
..
.. The components are connected together in application topologies.
.. To simplify topology creation, Ystia provides **topology templates** that can be extended by your applications.
..

**Ystia CSAR libray** provides a packaged solution to create easily Big Data application clusters on demand.
Deployment of Big Data applications can be done on a public Cloud (such as Amazon),
or on a private cloud (such as OpenStack), on Bare-Metal or on HPC.

Big Data applications targeted by Ystia are:

- **Log Analysis** applications based on Elastic_ components.
- message brokers (Kafka_, Nifi_),
- data science development environments (RStudio_, Jupyter_)
- and other technical components such as **Java**, **Consul** (Consensus Systems), allowing detailed application
  architectures to be designed.

The components are connected together in application topologies.
To simplify topology creation, Ystia provides **topology templates** that can be extended by your applications.

.. _Cloudera: https://www.cloudera.com/
.. _Consul: https://www.consul.io/
.. _Elastic: https://www.elastic.co/products
.. _Hortonworks: https://hortonworks.com/
.. _Jupyter: http://jupyter.org/
.. _Kafka: https://kafka.apache.org/
.. _MapR: https://mapr.com/
.. _MongoDB: https://www.mongodb.com/
.. _MySQL: http://www.mysql.com/
.. _Nifi: https://nifi.apache.org/
.. _PostgreSQL: https://www.postgresql.org/
.. _RStudio: https://www.rstudio.com/

Ystia is based on the following products:

- Alien4Cloud_, the interface for end-users and administrators. It allows you to define application architectures
  to be deployed on any Cloud.
- Janus_, the engine to orchestrate application deployment. It works for many Clouds and for Bare-Metal.

.. _Janus: http://TO_BE_COMPLETED/
.. _Alien4Cloud: http://alien4cloud.github.io/

**TO BE CONFIRMED .....** and **TO BE COMPLETED .....**



.. *********************************************************************************************************************
.. _getting_started_section:

***************
Getting Started
***************

    This section describes how to set up a basic application cluster using Ystia components.


.. _getting_started_requirements_section:

Requirements
============

YSTIA CSAR library requires:

- A running instance of **Janus** version **TO BE COMPLETED**
- A running instance of **Alien4Cloud** version **TO BE COMPLETED**
- The **Ystia CSAR Library** package, which provides components and topology templates to upload them in the
  Alien4Cloud catalog

**TO BE COMPLETED**

.. _getting_started_build_section:

How to build an Ystia CSAR
==========================

**TO BE COMPLETED**

.. _getting_started_samples_section:

Welcome sample
==============

The **Welcome** Ystia component is a very sample HTTP server.
It can be used to create and deploy your first Alien4Cloud application and to check the Ystia installation.

More information can be found under:

- **org/ystia/samples/welcome** and
- **org/ystia/samples/topologies/welcome_basic**

.. *********************************************************************************************************************

.. _topologies_section:

**********
Topologies
**********

    Ystia provides various topology templates, which can be used for demos, development or production applications.


.. _topologies_elk_section:

Topologies for Log Analysis based on Elastic Stack
==================================================

+-------------------+----------------------------------------------+
| **elk_basic**     | *org/ystia/topologies/elk_basic*             |
+-------------------+----------------------------------------------+
| **elk_broker**    | *org/ystia/topologies/elk_broker*            |
+-------------------+----------------------------------------------+
| **elk_ha**        | *org/ystia/topologies/elk_ha*                |
+-------------------+----------------------------------------------+
| **elk_geonames**  | *org/ystia/topologies/elk_geonames*          |
+-------------------+----------------------------------------------+

+-------------------+----------------------------------------------+
| **elk_beats**     | *org/ystia/samples/topologies/elk_beats*     |
+-------------------+----------------------------------------------+
| **elk_heartbeat** | *org/ystia/samples/topologies/elk_heartbeat* |
+-------------------+----------------------------------------------+
| **elk_dummylogs** | *org/ystia/samples/topologies/elk_dummylogs* |
+-------------------+----------------------------------------------+
| **elk_nifi**      | *org/ystia/samples/topologies/elk_nifi*      |
+-------------------+----------------------------------------------+
| **elk_twitter**   | *org/ystia/samples/topologies/elk_twitter*   |
+-------------------+----------------------------------------------+

Topologies for Flink
====================

+-----------+------------------------------+
| **flink** | *org/ystia/topologies/flink* |
+-----------+------------------------------+


.. *********************************************************************************************************************

.. _components_section:

**********
Components
**********


Consensus systems
=================

+------------+--------------------+
| **Consul** | *org/ystia/consul* |
+------------+--------------------+

ELK components
==============

+-------------------+---------------------------+
| **Elasticsearch** | *org/ystia/elasticsearch* |
+-------------------+---------------------------+
| **Logstash**      | *org/ystia/logstash*      |
+-------------------+---------------------------+
| **Kibana**        | *org/ystia/kibana*        |
+-------------------+---------------------------+
| **Beats**         | *org/ystia/beats*         |
+-------------------+---------------------------+


Geolocation components
======================

+--------------+----------------------+
| **GeoNames** | *org/ystia/logstash* |
+--------------+----------------------+


Social network connectors
=========================

+----------------------+----------------------+
| **TwitterConnector** | *org/ystia/logstash* |
+----------------------+----------------------+


Message brokers
===============

+-----------+-------------------+
| **Kafka** | *org/ystia/kafka* |
+-----------+-------------------+
| **Nifi**  | *org/ystia/nifi*  |
+-----------+-------------------+


Stream & real-time processing
=============================

+-----------+-------------------+
| **Flink** | *org/ystia/flink* |
+-----------+-------------------+


Studios for data scientists
===========================

+-------------+---------------------+
| **Jupyter** | *org/ystia/jupyter* |
+-------------+---------------------+
| **RStudio** | *org/ystia/rstudio* |
+-------------+---------------------+


Utilities
=========

+-------------+---------------------+
| **HAProxy** | *org/ystia/haproxy* |
+-------------+---------------------+
| **Java**    | *org/ystia/java*    |
+-------------+---------------------+
| **Python**  | *org/ystia/python*  |
+-------------+---------------------+
| **XFS**     | *org/ystia/xfs*     |
+-------------+---------------------+



.. *********************************************************************************************************************

.. _recovery_section:

********
Recovery
********

    This section describes how to recover manually Ystia components.
    This will be useful, for example, after a reboot of VMs that host Ystia components.

    The start/stop scripts of Ystia components are integrated as **services** into the Linux init system **systemd**.

Some Ystia components/services are automatically started at boot, while others are not.

Useful **systemd** basic commands:

- To start a service::

    $ sudo systemctl start <service-name>

- To stop a service::

    $ sudo systemctl stop <service-name>

- To get the status of a service, followed by most recent log data from the journal::

    $ sudo systemctl status <service-name>

- To show the messages for the service::

    $ journalctl -u <service-name>

  or::

    $ journalctl -u <service-name> --no-pager

Consul
======

The Consul component (agent and server) matches the **consul** systemd service.

The **consul** service is not started at boot.

The **consul** service corresponding to the server must be started first, then the **consul** services corresponding
to the agents can be started.

ELK and Kafka
=============

Elasticsearch
-------------

The Elasticsearch component matches the **elasticsearch** systemd service.

The **elasticsearch** service is not started at boot.

If the Elasticsearch component depends on a Consul agent, the associated **consul** service must be started first.

Logstash
--------

The Logstash component matches the **logstash** systemd service.

The **logstash** service is not started at boot.

If the Logstash component depends on a Consul agent, the associated **consul** service must be started first.

Kibana
------

The Kibana component matches two systemd services:

- **kibana** service
- **elasticsearch** service corresponding to the Elasticsearch client associated to Kibana.

When the **kibana** service is started, the **elasticsearch** service is automatically started.

When the **kibana** service is stopped, the **elasticsearch** service is not automatically stopped.

So, to start Kibana component, just start the **kibana** service. To stop Kibana component,
stop the **elasticsearch** service, then the **kibana** service .

The **kibana** service is not started at boot.

If the Kibana component depends on a Consul agent, the associated **consul** service must be started first.

Beats
-----

Each Beats component matches one systemd service :

- FileBeat: **filebeat** service
- PacketBeat: **packetbeat** service
- TopBeat: **topbeat** service

The beat services are not started at boot.

Kafka
-----

The Kafka component matches two systemd services:

- **zookeeper** service
- **kafka** service

To start Kafka component, start first the **zookeeper** service, then the **kafka** service.

To stop Kafka component, stop first the **kafka** service, then the **zookeeper** service.

The **zookeeper** and **kafka** services are not started at boot.

If the Kafka component depends on a Consul agent, the associated **consul** service must be started first.

For a Kafka cluster, **zookeeper** services must be started first on all the nodes of the cluster,
then **kafka** services can be started.

ELK topologies
--------------

For **elk-basic** topology, the start order of the services is the following:

- Start consul server on Compute_CS
- Start consul agents on Compute_ES, Compute_KBN, and Compute_LS
- Start elasticsearch service on Compute_ES
- Start kibana service on Compute_KBN (elasticsearch client service is automatically started)
- Sart logstash service on Compute_LS.

For **elk-broker** topology, the start order of the services is the following:

- Start consul server on Compute_CS
- Start consul agents on Compute_ES, Compute_KBN, Compute_KFK, Compute_LI and Compute_LS
- Start elasticsearch service on Compute_ES
- Start kibana service on Compute_KBN (elasticsearch client service is automatically started)
- Start zookeeper service, then kafka service on Compute_KFK
- Start logstash service on Compute_LI
- Start logstash service on Compute_LS.

For **elk-ha** topology:

- Mount the **LinuxFileSystem** on the nodes of Elasticsearch cluster and Kafka cluster. For example::

      $ sudo mount /dev/vdb1 /mountedStorageES
      $ sudo mount /dev/vdb1 /mountedStorageKFK

- Start services in the same order as for **elk-broker** topology except for Kafka cluster.
  Indeed, **zookeeper** services must be started first on all the nodes of the cluster,
  then **kafka** services can be started.

Studios for data scientists
===========================

RStudio
-------

The RStudio component matches the **rstudio-server** systemd service.

The **rstudio-server** service is automatically started at boot.

Jupyter
-------

The Jupyter component matches the **jupyter** systemd service.

The **jupyter** service is not started at boot.



.. *********************************************************************************************************************

.. _monitoring_and_troubleshooting_section:

****************************
Monitoring & troubleshooting
****************************

**TO BE COMPLETED ...**



.. *********************************************************************************************************************

.. _references_section:

**********
References
**********

Alien4Cloud documentation
  https://alien4cloud.github.io/#/documentation/1.4.0/index.html

Janus documentation
  https://TO_BE_COMPLETED


**TO BE COMPLETED.....**


