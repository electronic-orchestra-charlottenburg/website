.. title: Heavy Rotations
.. slug: heavy_rotations
.. date: 2019-05-27 22:44:21 UTC+02:00
.. tags:
.. category: repertoire
.. link:
.. description:
.. type: text


**2019** – for 2 turntables and 8 modular synths.

*Heavy Rotations* is a technical concept for a live electronic improvisation, relying on the use of time-code vinyl for the
integrated control of spatialization and modular synthesizers. This strong connection between spatial and timbral parameters
results in an enhanced spatialization experience.
Heavy Rotations is composed for the EOC, using 8 modular systems and two turntables.

.. figure:: /images/eoc_now_heavy_2.jpg
	:width: 600px

	*Heavy Rotations with the EOC, Copyright Dirk Rose*

-----------

Technical Concept
=================

The concept is based on an adopted version of the free timecode vinyl software `xwax <https://xwax.org/>`_,
as well as Puredata and SuperCollider. PD is used to generate LFO signals, which are sent to the modular systems
as control voltages (CV). These CV signals are patched to timbral parameters on the systems by the musicians.
The synth outputs are afterwards processed with a final VCA stage in SuperCollider
and finally spatialized.

.. figure:: /images/heavy_rotations_flow.png
	:width: 500px

	*Global setup for Heavy Rotations*

-----

The VCA, or gain modules, change the synthesizers' signals in amplitude, depending on
the LOFO signals:

.. figure:: /images/heavy_rotations_flow_2.png
	:width: 500px

	*Gain module (VCA) for a single synth.*

.....

Four basic LFO waveforms can be selected during the performance.
The piece starts with a soft sinusoidal modulation and moves towards
an aggressive square wave, ending in a constant signal.

.. figure:: /images/heavy_rotations_lfo.png
	:width: 600px

	*LFO waveforms.*

-----


Spatial Movements
=================

Heavy Rotations works with simple circular movements, orbiting the center of the listening space.
The speed of the rotation is directly linked to the spinning speed of the turntables.
This is a binaural rendering from a performance at Holzmarkt, Berlin, in 2019:


.. raw:: html

  <audio controls preload="none">
    <source src="/audio/HeavyRotations_Holzmarkt_2019.mp3" type="audio/mp3">
  </audio>
