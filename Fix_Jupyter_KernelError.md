## How to fix Jupyter Notebook Kernel Error

The reason that the kernel fails may be complicated. But the logic is that you have a different python version($which python), but the jupyter can not find that version. Thus it fails to talk to the python version that you're now using. The solution is that you let the current python install the ipykernel, and then make the ipykernel to be installed on the user.

Two lines of commands are important:
python -m pip install ipykernel
python -m ipykernel install --user(Hey Jupyter, I don't know what version of python you are using, but just connect to the version of python that I am using in the terminal.)

Some packages may not work as you installed them with previous versions of python. You have to reinstall them. However, this makes life easier compared to other solutions like uninstalling and reinstalling conda, or creating a new envirenment and moving all notebooks to that new kernel.

 

References:
https://www.youtube.com/watch?v=m0TLwkje6co
https://ipython.readthedocs.io/en/stable/install/kernel_install.html

