.. _elk_twitter_section:

***********
ELK_TWITTER
***********

.. contents::
    :local:
    :depth: 3

Install Components and Topology template
----------------------------------------
Install the CSARs of the following YSTIA compoents to the Alien4Cloud Components catalog, and respect the order in the list:

#. **common**
#. **consul**
#. **java**
#. **kafka**
#. **elasticsearch**
#. **logstash**

Install the **elk_twitter** topology archive to the Alien4Cloud Topology template catalog.


Topology template
-----------------
The **elk_twitter** template provides the following configuration:

- Relationships between the ELK components are created.

- ELK components are designed to be deployed on Compute hosts and appropriate Java distribution.

- Consul allows Elasticsearch cluster discovery.

- The twitter connector is hosted by the Logstash node

Create en application
---------------------
A Log Analysis application can be created via the Alien4Cloud GUI using the **elk_twitter** topology shown below:

.. image:: docs/images/elk_twitter_topo.png
   :name: elk_twitter_figure
   :scale: 100
   :align: center

Complete configuration
----------------------

- Create a **Kibana Dashboard** to present the specific data items corresponding to the application needs. You can find in the dashboards repository of this topology two Kibana dashboard samples : "fr_elections_2017.json" and "us_elections_2017.json"

- Configure the Twitter connector by setting values for properties consumer_key, consumer_secret, oauth_token, oauth_token_secret, use_proxy, proxy_address, proxy_port (sse README file in the Logstash component's source code)