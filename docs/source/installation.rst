Kurulum
=====

.. _installation:

Miniforge
------------

Windows
^^^^^^^^

Kullanıcı bilgisayarlarına mevcut temel sistem ayarları bozulmadan, yeni ortam oluşturularak kurulum
yapılmalıdır. Bu iş için ilk olarak sanal ortam kurulur. https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Windows-x86_64.exe adresinden Windows için kurulum dosyası indirilir ve ardından varsayılan ayarlar ile kurulum yapılır. “Sadece benim için kur” seçeneği seçilirse (tercihen) kurulum C:\Users
altına gerçekleşir. Örneğin benim bilgisayarımda C:\Users\murat\miniforge3 altında kurulum
sorunsuz çalışmaktadır.

Linux
^^^^^^^^

https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-x86_64.sh

.. code-block:: console
bash Miniforge3-Linux-x86_64.sh
eval "$(/home/murat/miniforge3/bin/conda shell.bash hook)"
conda init
conda config --set auto_activate_base false

OsX
^^^^^^^^

https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-MacOSX-x86_64.sh

.. code-block:: console
bash Miniforge3-MacOSX-x86_64.sh

uhte Yeni Ortam Kurulumu
------------

JupyterLab
------------

GNU Radio
------------


Kütüphaneler
------------

osmocom
------------

RTL-SDR Sürücüleri
------------

Kurulumun Testi
------------

