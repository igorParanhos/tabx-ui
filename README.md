# README.md

## Kivy instructions

Kivy will need to know where the SDL dependencies are installed. To do so, you must set the KIVY_DEPS_ROOT environment variable to the path of the kivy-dependencies directory. For example, if you are in the kivy-deps-build directory, you can set the environment variable with:

```shell
export KIVY_DEPS_ROOT=$(pwd)/kivy-dependencies
```
With the dependencies installed, and KIVY_DEPS_ROOT set you can now install Kivy into the virtual environment.

To install the stable version of Kivy, from the terminal do:

python -m pip install "kivy[base]" kivy_examples --no-binary kivy
To install the latest cutting-edge Kivy from master, instead do:

python -m pip install "kivy[base] @ https://github.com/kivy/kivy/archive/master.zip"