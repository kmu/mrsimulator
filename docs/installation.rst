

.. _shielding_tensor_api:

============
Installation
============

The `mrsimulator` package requires the `fftw3 <https://anaconda.org/eumetsat/fftw3>`_
C routines to function. Download and install the fftw3 by typing the following
in the terminal

.. code-block:: python

    conda install -c eumetsat fftw3


Additionally, ``mrsimulator`` requires the following packages.

 - `NumPy <http://www.numpy.org>`_
 - `SciPy <https://www.scipy.org>`_
 - `astropy <https://www.astropy.org>`_
 - mkl, mkl-include

You may install these package using pip as

.. code-block:: python

    pip install numpy scipy astropy mkl mkl-include

For figures and visualization, we use the following packages.

 - `plotly <https://plot.ly/python/>`_
 - dash
 - dash_daq

To install these package use

.. code-block:: python

    pip install matplotlib plotly dash dash_daq


Finally to install the ``mrsimulator`` package, type the following
in the terminal

.. code-block:: python

    pip install git+https://github.com/DeepanshS/mrsimulator.git@master



Test
++++

If the installation is successful, you should be able to run the following
in the terminal.

.. code-block:: python

    python -c "import mrsimulator; mrsimulator.run_test()"

This will display the following message on the screen

.. code-block:: python

    Setting up the virtual NMR spectrometer
    ---------------------------------------
    Adjusting the magnetic flux density to 9.4 T.
    Setting rotation angle to 0.9553059660790962 rad.
    Setting rotation frequency to 0.0 Hz.
    Detecting 1H(I=0.5, precession frequency = 400.228301848 MHz) isotope.
    Recording 1H spectrum with 2048 points over a 25000.0 Hz bandwidth and a reference offset of 0.0 Hz.
    <BLANKLINE>
    1H site 0 from isotopomer 0 @ 100.0% abundance
    ----------------------------------------------
    isotropic chemical shift = 0.0 ppm
    chemical shift anisotropy = 13.89 ppm
    chemical shift asymmetry = 0.25
    Setting up the virtual NMR spectrometer
    ---------------------------------------
    Adjusting the magnetic flux density to 9.4 T.
    Setting rotation angle to 0.9553059660790962 rad.
    Setting rotation frequency to 1000.0 Hz.
    Detecting 1H(I=0.5, precession frequency = 400.228301848 MHz) isotope.
    Recording 1H spectrum with 2048 points over a 25000.0 Hz bandwidth and a reference offset of 0.0 Hz.
    <BLANKLINE>
    1H site 0 from isotopomer 0 @ 100.0% abundance
    ----------------------------------------------
    isotropic chemical shift = 0.0 ppm
    chemical shift anisotropy = 13.89 ppm
    chemical shift asymmetry = 0.25

and a corresponding plot shown below.

.. image:: /_static/test_output.pdf
