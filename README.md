# Troubleshooting ORTOOLS

The simple way of installing google's `ortools` using `pip install ortools` doesn't work on windows.

e.g.
```shell
# Powershell
python -m venv venv # using python 3.12.3
pip install ortools
# Copy example from employee scheduling problem name it as nurses.py
## https://developers.google.com/optimization/scheduling/employee_scheduling
python nurse.py # No output
```

On troubleshooting, u will realise that the code breaks when calling `cp.solve()`


## Potential solution




1. Microsoft Visual C++ Redistributable


1. install runtime from https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170
   nope. doesn't work

1. Explained on developers.google.com

   https://developers.google.com/optimization/install/python/pkg_windows
    
   https://visualstudio.microsoft.com/downloads/?q=Visual+C%2B%2B+Redistributable+for+Visual+Studio



