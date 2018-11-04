#### An instruction for installing TAMkin 1.2.4 on your Windows PC

First of all I make a apology for neglect of updating [TAMkin for Windows](https://github.com/brhr-iwao/TAMkin_for_Windows/).
A reason why is absent of freely available Windows installers of Scipy 0.17.1 and Numpy 1.6.2 or later, which are [TAMkin 1.2.4](https://github.com/molmod/tamkin/releases/tag/1.2.4) dependencies.
To build the Numpy installer by oneself, [Intel MKL](https://software.intel.com/en-us/mkl) is required and I don't have it !

Instead of providing the latest binary of TAMKin for Windows, I show a way to install [TAMkin 1.2.4](https://github.com/molmod/tamkin/releases/tag/1.2.4) on your Windows PC by using Python  [pip](https://pypi.org/project/pip/).  
If you have a Windows PC connecting to the internet, you can install [TAMkin 1.2.4](https://github.com/molmod/tamkin/releases/tag/1.2.4) by following the instruction to be described. (Off course free of charge !)

1. If [Python](https://www.python.org/) for Windows have not been installed on your Windows PC, download and install [Python for Windows](https://www.python.org/downloads/windows/).  
Download a [Python 2.7.9 installer](https://www.python.org/downloads/release/python-279/) or later for Windows and install it on your Windows PC. Off course you can use Python 3.  
A Windows installer of [Python 2.7.9](https://www.python.org/downloads/release/python-279/) or later (or off course Python 3) installs [pip](https://pypi.org/project/pip/) with default settings.  
Assume we use Python 2.7.14 for example after this.
2. Download and install the dependencies.  
In accordance with your Python environment, download and install the dependencies. Here I described the case used the latest version at October 2018 for Python 2.7.  

  2-1. Download and install Numpy.  
  Download numpy‑1.14.6+mkl‑cp27‑cp27m‑win32.whl from ["Unofficial Windows Binaries for Python Extension Packages"(https://www.lfd.uci.edu/~gohlke/pythonlibs/)](https://www.lfd.uci.edu/~gohlke/pythonlibs/) and save it on your PC. If you have other version than Python 2.7, download a appropriate wheel package.  
  Launch the Windows command prompt and type the following command (replacing "C:\Your_Saved_Directory" with the true directory path):  

  >  python -m pip install C:\Your_Saved_Directory\numpy‑1.14.6+mkl‑cp27‑cp27m‑win32.whl


  Installation is successfully completed if you see the following message:

  > Installing collected packages: numpy  
  > Successsfully installed numpy-1.14.6+mkl  


  2-2. Download and Install Scipy.  
  Download scipy‑1.1.0‑cp27‑cp27m‑win32.whl from ["Unofficial Windows Binaries for Python Extension Packages"(https://www.lfd.uci.edu/~gohlke/pythonlibs/)](https://www.lfd.uci.edu/~gohlke/pythonlibs/) and save it on your PC. If you have other version than Python 2.7, download a appropriate wheel package.  
  Type the following command (replacing "C:\Your_Saved_Directory" with the true directory path) on the Windows command prompt:  

  >  python -m pip install C:\Your_Saved_Directory\scipy‑1.1.0‑cp27‑cp27m‑win32.whl


    Installation is successfully completed if you see the following message:

    > Installing collected packages: scipy  
    > Successfully installed scipy-1.1.0   


  2-3. Install Matplotlib  
    Type the following command (replacing "C:\Your_Saved_Directory" with the true directory path) on the Windows command prompt:  

    >  python -m pip install matplotlib   


    The dependencies, a.k.a. [kiwisolver](https://files.pythonhosted.org/packages/6d/c5/ca9bbf1249119900e53996ed1530f073a7ada3946495231eb92a6f1f737c/kiwisolver-1.0.1-cp27-none-win32.whl), [pyparsing](https://files.pythonhosted.org/packages/2b/4a/f06b45ab9690d4c37641ec776f7ad691974f4cf6943a73267475b05cbfca/pyparsing-2.2.2-py2.py3-none-any.whl), [backports.functools-lru-cache](https://files.pythonhosted.org/packages/03/8e/2424c0e65c4a066e28f539364deee49b6451f8fcd4f718fefa50cc3dcf48/backports.functools_lru_cache-1.5-py2.py3-none-any.whl), [six](https://files.pythonhosted.org/packages/67/4b/141a581104b1f6397bfa78ac9d43d8ad29a7ca43ea90a2d863fe3056e86a/six-1.11.0-py2.py3-none-any.whl), [pytz](https://files.pythonhosted.org/packages/30/4e/27c34b62430286c6d59177a0842ed90dc789ce5d1ed740887653b898779a/pytz-2018.5-py2.py3-none-any.whl), [cycler](https://files.pythonhosted.org/packages/f7/d2/e07d3ebb2bd7af696440ce7e754c59dd546ffe1bbe732c8ab68b9c834e61/cycler-0.10.0-py2.py3-none-any.whl) and  [python-dateutil](https://files.pythonhosted.org/packages/cf/f5/af2b09c957ace60dcfac112b669c45c8c97e32f94aa8b56da4c6d1682825/python_dateutil-2.7.3-py2.py3-none-any.whl) will be installed with [matplotlib](https://files.pythonhosted.org/packages/6e/cf/0153fe3767addefdd8bc81e7f41143477a8528ddec64544ef35d06f9a38a/matplotlib-2.2.3-cp27-cp27m-win32.whl).  
    You can install matplotlib on a stand-alone PC after installing these dependencies one by one with "python -m pip install the_wheel_name" commands.  

  2-4. Download and install Cython.  
    Download Cython‑0.28.5‑cp27‑cp27m‑win32.whl from ["Unofficial Windows Binaries for Python Extension Packages"(https://www.lfd.uci.edu/~gohlke/pythonlibs/)](https://www.lfd.uci.edu/~gohlke/pythonlibs/) and save it on your PC. If you have other version than Python 2.7, download a appropriate wheel package.  
    Type the following command (replacing "C:\Your_Saved_Directory" with the true directory path) on the Windows command prompt:  

    >  python -m pip install C:\Your_Saved_Directory\Cython-0.28.5-cp27-cp27m-win32.wh  


      Installation is successfully completed if you see the following message:

      > Installing collected packages: Cython  
      > Successfully installed Cython-0.28.5   


    2-5. Install [molmod](https://github.com/molmod/molmod).  
      Type the following command (replacing "C:\Your_Saved_Directory" with the true directory path) on the Windows command prompt:  

      >  python -m pip install molmod   


      The dependencies, a.k.a. [nose](https://files.pythonhosted.org/packages/99/4f/13fb671119e65c4dce97c60e67d3fd9e6f7f809f2b307e2611f4701205cb/nose-1.3.7-py2-none-any.whl) and [future](https://files.pythonhosted.org/packages/00/2b/8d082ddfed935f3608cc61140df6dcbf0edea1bc3ab52fb6c29ae3e81e85/future-0.16.0.tar.gz) will be installed with [molmod](https://files.pythonhosted.org/packages/89/80/6a23f730196ed3ffb478dc3f9ea047913c99091d301cc82f4820ecee095d/molmod-1.4.4.tar.gz).  
      You can install matplotlib on a stand-alone PC after installing these dependencies one by one with "python -m pip install the_wheel_name" commands.  

    2-6. Install [TAMkin 1.2.4](https://github.com/molmod/tamkin/releases/tag/1.2.4)  
      The "python -m pip install tamkin" command did not work in my experience. So download [TAMkin 1.2.4](https://files.pythonhosted.org/packages/51/03/4e9e3a050306849da3d20d4142806a6c58ab72763da25f6c85529c505b6a/tamkin-1.2.4.tar.gz), save and expand it with a file expander such as [7-zip](https://www.7-zip.org/).  
      Change the currnet directory to "taamkin-1.2.4" (the directory which contains setup.py) and type the following command (replacing "C:\Your_Saved_Directory" with the true directory path) on the Windows command prompt:

      > python setup.py install   


   3. Testing  
   You can test TAMkin with Python scripts in  tankin-1.2.4\tamkin\examples.  
   For example, change the current directory to "tamkin-1.2.4\tamkin\exaamples\001_ethane\" on the Windows command prompt and execute the following command:
   > python thermo.py  

   If TAMkin is correctly installed, "partfun.txt" and "thermo.csv" will be generated in this directory.

   4. Uninstallation  
   From Windows "Settings" > "Apps", you can uninstall these python packages and python one by one.  

   Happy computing !
