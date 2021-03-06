.. Images
.. |dht11_1| image:: images/dht11_1.jpg

.. Links
.. |plugin_development| raw:: html

   <a href="../../plugin_developers_guide/03_south_C_plugins.html">plugin development</a>

.. |python_version| raw:: html

   <a href="../fledge-south-dht11/index.html">Python version</a>

DHT11 (C version)
=================

.. image:: images/dht11.jpg
   :align: right

The *fledge-south-dht* plugin implements a temperature and humidity sensor using the DHT11 sensor module. Two versions of plugins for the DHT11 are available and are used as the example for |plugin_development|. The other DHT11 plugin is *fledge-south-dht11* and is a |python_version|.

The DHT11 and the associated DHT22 sensors may be used, however they have slightly different characteristics;

+--------------------+-----------------------------+-------------------------------+
|                    | DHT11                       | DHT22                         |
+====================+=============================+===============================+
| Voltage            | 3 to 5 Volts                | 3 to 5 Volts                  |
+--------------------+-----------------------------+-------------------------------+
| Current            | 2.5mA                       | 2.5mA                         |
+--------------------+-----------------------------+-------------------------------+
| Humidity Range     | 0-50 % humidity 5% accuracy | 0-100% humidity 2.5% accuracy |
+--------------------+-----------------------------+-------------------------------+
| Temperature Range  | 0-50 +/- 2 degrees C        | -40 to 80 +/- 0.5 degrees C   |
+--------------------+-----------------------------+-------------------------------+
| Sampling Frequency | 1Hz                         | 0.5Hz                         |
+--------------------+-----------------------------+-------------------------------+

.. note::

   Due to the requirement for attaching to GPIO pins this plugin is only available for the Raspberry Pi platform.

To create a south service with the DHT11 plugin

  - Click on *South* in the left hand menu bar

  - Select *dht11_V2* from the plugin list

  - Name your service and click *Next*

  +-----------+
  | |dht11_1| |
  +-----------+

  - Configure the plugin

    - **Asset Name**: The asset name which will be used for all data read.

    - **Rpi Pin**: The GPIO pin on the Raspberry Pi to which the DHT11 serial pin is connected.

  - Click *Next*

  - Enable the service and click on *Done*

