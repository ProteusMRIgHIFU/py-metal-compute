# Modified
# metalcompute for Python - modified 
  Disclaimer: Please consult https://github.com/baldand/py-metal-compute for the official `py-metal-compute` library. In this version, we modified the original `py-metal-compute` for a multi GPU backend project (https://github.com/ProteusMRIgHIFU/BabelViscoFDTD) to add some features we really need. Mostly being able to modify regions of buffers, choose between shared and managed modes in buffers (which is critical to have decent performance in both M1-M2 and old AMD processors in X64 systems) and more granular control of commits to dispatch an execution. Because these changes break pretty much how the original `py-metal-compute` library works, that is why we decided to change the name of the installation library to avoid any conflict with any existing use of `py-metal-compute`. We really thank @baldand for the amazing work. It really helped us a lot. Feel free to explore our changes and hopefully they may be useful for other people.


## Installation
To avoid confusion with the original,  this modified version can be installed via
`pip install git+https://github.com/ProteusMRIgHIFU/py-metal-compute.git`
Please note the library will be installed with the name of `metalcomputebabel` to avoid conflicts with the original, which installs as `metalcompute`.
