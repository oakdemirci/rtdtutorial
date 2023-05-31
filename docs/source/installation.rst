Kurulum
=====

.. _installation:

Miniforge
------------

Windows
^^^^^^^^


.. note::

   Installation should be completed using a new virtual environment, without changing current system settings.


First create a new virtual environment.
Download `miniforge`_ file and run executable. Installation for current user is recommended and the target will be c:\\Users directory, for example the app will run from c:\\Users\\murat\\miniforge3 directory after a successful installation.

.. _miniforge: https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Windows-x86_64.exe

Linux
^^^^^^^^

`Linux kurulum`_ dosyası indirilir.

.. _linux kurulum: https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-x86_64.sh

.. code-block:: console

   bash Miniforge3-Linux-x86_64.sh
   eval "$(/home/murat/miniforge3/bin/conda shell.bash hook)"
   conda init
   conda config --set auto_activate_base false

OsX
^^^^^^^^

`OsX kurulum`_ dosyası indirilir.

.. _osx kurulum: https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-MacOSX-x86_64.sh

.. code-block:: console

   bash Miniforge3-MacOSX-x86_64.sh

UHTE Yeni Ortam Kurulumu
------------

.. note::

   Windows işletim Sisteminde; Miniforge kurulduktan sonra Windows tuşuna basılarak, “miniforge” aratıldığında “Miniforge Prompt” komut satırı görüntülenmektedir. Miniforge Prompt açılarak eğitim boyunca kullanacağımız UHTE ortamı aşağıdaki komut yazılarak oluşturulur.


.. code-block:: console

   conda create -vv -n UHTE python=3.9 jupyter


JupyterLab
------------

Ardından aynı “Miniforge Prompt” ekranında ilk olarak UHTE ortamı aktive edilir ve JupyterLab uygulaması kurulur.

.. code-block:: console

   conda activate UHTE
   conda install jupyterlab


GNU Radio
------------

Aynı ekranda aşağıdaki komutlar ile GNU Radio kurulur.

.. code-block:: console

   conda config --append channels conda-forge
   conda install gnuradio python=3.9


Kütüphaneler
------------

Aynı ekranda aşağıdaki komutlar ile ilgili Python kütüphaneleri kurulur.

.. code-block:: console

   conda install numpy
   conda install scipy
   conda install matplotlib
   conda install -c conda-forge ipympl
   conda install -c conda-forge python-sounddevice
   pip install playsound==1.2.2
   conda install soapysdr-module-rtlsdr
   conda install pymodes


osmocom
------------

`Osmocom`_ kurulumu indirilir ve conda ortamı (UHTE) altına çıkarılır. (Örneğin C:\Users\murat\miniforge3\envs\UHTE)

.. _osmocom: https://downloads.osmocom.org/binaries/windows/rtl-sdr/rtl-sdr-64bit-20221120.zip

RTL-SDR Sürücüleri
------------

`Rtl`_ ve `Sdr`_ kurulumları indirilir.

.. _rtl: https://github.com/pbatard/libwdi/releases/download/b730/zadig-2.5.exe
.. _sdr: https://airspy.com/?ddownload=3130

Sürücü kurulumu gerçek donanıma ihtiyaç duyduğu için ders esnasında gerçekleştirilecektir.
Yukarıdaki dosyaların kullanıcı bilgisayarına indirilmesi yeterlidir.


Kurulumun Testi
------------

Kurulumları test etmek için yeni bir Miniforge Prompt açılır ve komut satırından UHTE ortamı
aktive edilir ve ardından Jupyter Lab başlatılır.

.. code-block:: console

   conda activate UHTE
   jupyter-lab

Gelen Launcher ekranından Python3 Notebook seçilerek yeni bir not defteri oluşturulur.
