Dependencies
=========

The role dependencies allows you to install dependencies default for server.

Requirements
------------

For the proper functioning of the role, you will have to create a `main.yml` file and copy the information from `main.example` and fill in the information in it.

Role Variables
--------------

````yml
dependencies:
  - 'apt-transport-https'
  - 'ca-certificates'
  - 'curl'
  - 'software-properties-common'
  - 'python3-pip'
  - 'virtualenv'
  - 'python3-setuptools'
  - 'aptitude'
````

Author Information
------------------
* **DUMONT Baptiste** _alias_ [@BaptDu](https://github.com/BaptDu)
