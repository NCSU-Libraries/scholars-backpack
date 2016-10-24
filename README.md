# Scholar's Backpack

Modern research practice asks researchers to engage with information in new ways through the use of a rapidly changing array of digital technologies. The Scholar’s Backpack will bring together a sampler of commonly used digital tools that support the research lifecycle in one virtual machine, both decreasing the overhead of locating, installing, and learning how to use new tools and improving the reproducibility of scientific computing environments.

## Getting Started

1. Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads) and [Vagrant](https://www.vagrantup.com/downloads.html). **Vagrant 1.8.4 or higher is required.** **Windows users must also install a shell environment** like [Git for Windows](https://git-for-windows.github.io/).
1. Clone or download this repository as a zip file.
1. From a terminal application, navigate to the Python-Vagrant directory, type `vagrant up`, and hit the `Return` key.
1. Once Vagrant is finished, type `vagrant ssh` to access the virtual environment. This environment has been configured to automatically change the directory to `/vagrant/code` on the guest machine.

## Running the Introductory Jupyter Notebook

1. Using the GUI, select "Welcome to the Scholar's Backpack" from the desktop icons. This will open a Jupyter notebook that will walk you through the environment.

## What's inside?

### What this environment includes:

#### python role

* git
* vim
* build-essential
* python3
* python3-dev
* python3-setuptools
* python3-matplotlib
* python3-numpy
* python3-scipy
* python3-pandas
* python3-pil
* pip3
* beautifulsoup4
* requests
* wordcloud
* jupyter
* sympy
* nose

#### R role

* R
  * R-core
  * R-core-devel
* RStudio

##### R packages

- boot
- class
- cluster
- codetools
- foreign
- KernSmooth
- lattice
- MASS
- Matrix
- mgcv
- nlme
- nnet
- rpart
- spatial
- survival
- datasets

## Vagrant Notes

* The username and password on the guest are both `vagrant`. If the GUI switches to the lock screen, use `vagrant` as the password to login.
* To exit the guest environment, type `exit` from the command line anywhere in the guest.
* To shut down the virtual machine, type `vagrant halt` from within the Python-Vagrant directory on the host.
* To turn on the virtual machine, type `vagrant up` from within the Python-Vagrant directory on the host.
* For more detailed information, visit the [Vagrant Documentation](https://www.vagrantup.com/docs/)
