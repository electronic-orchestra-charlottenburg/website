.. title: S-Tog (Marc Applebaum)
.. slug: s-tog
.. date: 2021-11-15
.. tags:
.. category: adaption
.. link:
.. description:
.. type: text
.. priority: 0


`S-Tog <http://www.markapplebaum.com/stog.html>`_ is a graphic score with text instructions, composed by Marc Applebaum in 1991. The piece has been adapted for the EOC in a spatialized version. S-Tog uses a map of the Copenhagen metro system, replacing the station names with musical instructions. When performed, musicians can travel the network, implementing the different instructions which are based on their route:

.. figure:: /images/stog_2.gif
	   :width: 500

	   *Map from the S-Tog Score.*

----

EOC Version
===========

Path Selection
--------------

For the EOC, nine performers pick a path before the performance.
The only directive is that they should start at the boundaries of the network and pick a final station at the center.
These are the stations of two players (direction=top->bottom):

.. code-block:: console

    PLAYER 3                PLAYER 2

    H	Background            E	Loud
    F	Accelerando           E	ABA
    F	Decelerando           L	Minor
    F	ABA                   L	0,2,4
    B	Antithesis            E	High
    B	Loud                  E	Quiet
    B	Don´t Listen          E	Timbre


-----


Spatial Movements
-----------------

During the performance, each musician's sound is connected to a virtual sound source in the plane.
These virtual sound sources follow the path defined by the selected stations with rigid timing.
A Python sequencer takes care of processing the sequences of stations, converting them into spatial trajectories
and sending them to the audio rendering server.
This results in a continuously changing spatial arrangement of the virtual sound sources and thus
of the overall spatial sound image. This recording shows the whole process
of source movements with tenfold speed:


.. raw:: html

     <video width="800" controls src="/videos/s-tog-fast.mp4"></video>

*Source movements in tenfold speed.*


-----

Instructions
--------------

The instructions at the stations on the individual routes are presented to the musicians on screen,
synchronous to the source movements. This is realized with PyQT.
An additional pitch tracker is included to help getting the modular
systems in tune:

.. figure:: /images/s-tog-instructions.png
	   :width: 500

	   *S-Tog instructions.*

-----

Binaural Rendering
==================

This is a binaural rendering from a performance of S-Tog with the EOC,
during the festival *NOW!* in Essen (2019):

.. raw:: html

 <audio controls preload="none">
   <source src="/audio/EOC-Essen_Stog.mp3" type="audio/mp3">
 </audio>

\

.. figure:: /images/eoc-essen.jpg
	   :width: 600

*EOC at NOW! festival, Essen (2019).*
