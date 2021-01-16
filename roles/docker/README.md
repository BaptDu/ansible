Docker
=========

The role docker allows you to install dependencies and set up images automatically.

Requirements
------------

For the proper functioning of the role, you will have to create a `main.yml` file and copy the information from `main.example` and fill in the information in it.

Role Variables
--------------

````yml
registry: Url of the registry 
username: Username of the registry
password: Password of the registry
containers:
  - { 
    image: url of your image,
    version: lasted or name of your image vesion,
    name: name of your container  ,
    ports: ports to be published ex: "80:80"
    }
  # ...
````

Author Information
------------------
* **DUMONT Baptiste** _alias_ [@BaptDu](https://github.com/BaptDu)
