# Scholar's Backpack

Modern research practice asks researchers to engage with information in new ways through the use of a rapidly changing array of digital technologies. The Scholar’s Backpack brings together a sampler of commonly used scientific computing tools into one virtual machine, both decreasing the overhead of locating, installing, and learning how to use new tools and improving the reproducibility of scientific computing environments.

## Getting Started

1. Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads) and [Vagrant](https://www.vagrantup.com/downloads.html).
    * **Vagrant 1.9.2 or higher is required.**
    * **Windows users must also install a shell environment** like [Git for Windows](https://git-for-windows.github.io/).
1. Clone or download this repository as a zip file.

1. From a terminal application, navigate to the scholars-backpack directory, type `vagrant up`, and hit the `Return` key.

1. Once Vagrant is finished, type `vagrant ssh` to access the virtual environment. This environment has been configured to automatically change the directory to `/vagrant/code` on the guest machine.

## Running the Introductory Jupyter Notebook

Jupyter notebooks are accessible from [localhost:5453](http://localhost:5453)

## R Studio

R Studio is accessible from [localhost:5452](http://localhost:5452)

Username: `vagrant` Password: `vagrant`

## What's inside?

### Python

This environment uses [Anaconda 4.3.0](https://www.continuum.io/downloads) to install and manage Python. A complete list of included packages can be found under the [Python 3.6](https://docs.continuum.io/anaconda/pkg-docs) package list.

### R

Anaconda is also used to manage R. This environment uses the conda package [r-essentials](https://docs.continuum.io/anaconda/r-language-pkg-docs).

The following additional packages are installed using CRAN:

* plotly

## Vagrant Notes

* To exit the guest environment, type `exit` from the command line anywhere in the guest.
* To shut down the virtual machine, type `vagrant halt` from within the scholars-backpack directory on the host.
* To turn on the virtual machine, type `vagrant up` from within the scholars-backpack directory on the host.
* For more detailed information, visit the [Vagrant Documentation](https://www.vagrantup.com/docs/)
