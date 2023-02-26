# pipcontrol

This is a python module pip controller package

This package is developed for using pip module in python code

## How to work

get list of installed packages from pip list

check package is installed and installing package if not installed

## How to use

```python
import pipcontrol
# python_cmd : optional

pipcontrol.install(package_names=["package1", "package2"], python_cmd="python3.10")
pipcontrol.update(package_names=["package1", "package2"], python_cmd="python3.10")
pipcontrol.uninstall(package_names=["package1", "package2"], python_cmd="python3.10")

from os.path import dirname, abspath

ABS_PATH = dirname(abspath(__file__))

pipcontrol.requirement_freeze(abs_path=ABS_PATH, python_cmd="python3.10")
pipcontrol.requirement_install(abs_path=ABS_PATH, python_cmd="python3.10")
pipcontrol.requirement_uninstall(abs_path=ABS_PATH, python_cmd="python3.10")

```
