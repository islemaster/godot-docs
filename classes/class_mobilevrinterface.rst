.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the MobileVRInterface.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_MobileVRInterface:

MobileVRInterface
=================

**Inherits:** :ref:`ARVRInterface<class_arvrinterface>` **<** :ref:`Reference<class_reference>` **<** :ref:`Object<class_object>`

**Category:** Core

Brief Description
-----------------

Generic mobile VR implementation

Member Functions
----------------

+----------------------------+-------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`  | :ref:`get_display_to_lens<class_MobileVRInterface_get_display_to_lens>` **(** **)** const                                     |
+----------------------------+-------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`  | :ref:`get_display_width<class_MobileVRInterface_get_display_width>` **(** **)** const                                         |
+----------------------------+-------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`  | :ref:`get_iod<class_MobileVRInterface_get_iod>` **(** **)** const                                                             |
+----------------------------+-------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`  | :ref:`get_k1<class_MobileVRInterface_get_k1>` **(** **)** const                                                               |
+----------------------------+-------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`  | :ref:`get_k2<class_MobileVRInterface_get_k2>` **(** **)** const                                                               |
+----------------------------+-------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`  | :ref:`get_oversample<class_MobileVRInterface_get_oversample>` **(** **)** const                                               |
+----------------------------+-------------------------------------------------------------------------------------------------------------------------------+
| void                       | :ref:`set_display_to_lens<class_MobileVRInterface_set_display_to_lens>` **(** :ref:`float<class_float>` display_to_lens **)** |
+----------------------------+-------------------------------------------------------------------------------------------------------------------------------+
| void                       | :ref:`set_display_width<class_MobileVRInterface_set_display_width>` **(** :ref:`float<class_float>` display_width **)**       |
+----------------------------+-------------------------------------------------------------------------------------------------------------------------------+
| void                       | :ref:`set_iod<class_MobileVRInterface_set_iod>` **(** :ref:`float<class_float>` iod **)**                                     |
+----------------------------+-------------------------------------------------------------------------------------------------------------------------------+
| void                       | :ref:`set_k1<class_MobileVRInterface_set_k1>` **(** :ref:`float<class_float>` k **)**                                         |
+----------------------------+-------------------------------------------------------------------------------------------------------------------------------+
| void                       | :ref:`set_k2<class_MobileVRInterface_set_k2>` **(** :ref:`float<class_float>` k **)**                                         |
+----------------------------+-------------------------------------------------------------------------------------------------------------------------------+
| void                       | :ref:`set_oversample<class_MobileVRInterface_set_oversample>` **(** :ref:`float<class_float>` oversample **)**                |
+----------------------------+-------------------------------------------------------------------------------------------------------------------------------+

Member Variables
----------------

  .. _class_MobileVRInterface_display_to_lens:

- :ref:`float<class_float>` **display_to_lens** - The distance between the display and the lenses inside of the device in centimeters.

  .. _class_MobileVRInterface_display_width:

- :ref:`float<class_float>` **display_width** - The width of the display in centimeters.

  .. _class_MobileVRInterface_iod:

- :ref:`float<class_float>` **iod** - The interocular distance, also known as the interpupillary distance. The distance between the pupils of the left and right eye.

  .. _class_MobileVRInterface_k1:

- :ref:`float<class_float>` **k1** - The k1 lens factor is one of the two constants that define the strength of the lens used and directly influences the lens distortion effect.

  .. _class_MobileVRInterface_k2:

- :ref:`float<class_float>` **k2** - The k2 lens factor, see k1.

  .. _class_MobileVRInterface_oversample:

- :ref:`float<class_float>` **oversample** - The oversample setting. Because of the lens distortion we have to render our buffers at a higher resolution then the screen can natively handle. A value between 1.5 and 2.0 often provides good results but at the cost of performance.


Description
-----------

This is a generic mobile VR implementation where you need to provide details about the phone and HMD used. It does not rely on any existing framework. This is the most basic interface we have. For the best effect you do need a mobile phone with a gyroscope and accelerometer.

Note that even though there is no positional tracking the camera will assume the headset is at a height of 1.85 meters.

Member Function Description
---------------------------

.. _class_MobileVRInterface_get_display_to_lens:

- :ref:`float<class_float>` **get_display_to_lens** **(** **)** const

Returns the distance between the display and the lens.

.. _class_MobileVRInterface_get_display_width:

- :ref:`float<class_float>` **get_display_width** **(** **)** const

Return the width of the LCD screen of the device.

.. _class_MobileVRInterface_get_iod:

- :ref:`float<class_float>` **get_iod** **(** **)** const

Returns the interocular distance.

.. _class_MobileVRInterface_get_k1:

- :ref:`float<class_float>` **get_k1** **(** **)** const

Returns the k1 lens constant.

.. _class_MobileVRInterface_get_k2:

- :ref:`float<class_float>` **get_k2** **(** **)** const

Retuns the k2 lens constant

.. _class_MobileVRInterface_get_oversample:

- :ref:`float<class_float>` **get_oversample** **(** **)** const

Returns the oversampling setting.

.. _class_MobileVRInterface_set_display_to_lens:

- void **set_display_to_lens** **(** :ref:`float<class_float>` display_to_lens **)**

Sets the distance between display and the lens.

.. _class_MobileVRInterface_set_display_width:

- void **set_display_width** **(** :ref:`float<class_float>` display_width **)**

Sets the width of the LCD screen of the device.

.. _class_MobileVRInterface_set_iod:

- void **set_iod** **(** :ref:`float<class_float>` iod **)**

Sets the interocular distance.

.. _class_MobileVRInterface_set_k1:

- void **set_k1** **(** :ref:`float<class_float>` k **)**

Sets the k1 lens constant.

.. _class_MobileVRInterface_set_k2:

- void **set_k2** **(** :ref:`float<class_float>` k **)**

Sets the k2 lens constant.

.. _class_MobileVRInterface_set_oversample:

- void **set_oversample** **(** :ref:`float<class_float>` oversample **)**

Sets the oversampling setting.


