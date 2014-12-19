Facette
=======

[Facette](https://facette.io/) is a web application to display time series data from various sources on graphs, designed to be easy to setup and to use.
To learn more on its architecture, read [this page](http://docs.facette.io/architecture/).

Configuration
--------------

### Inventory

```ini
[collector:children]
collector-somedc-prod

[collector-somedc-prod]
collector1  ansible_ssh_host=172.16.0.120

[collector-somedc-prod:vars]

# Set this variable to true to install Facette.
# False by default.
use_facette = true

# The port Facette should listen on.
facette_port = 12003
```

See also
--------

* [Facette](https://facette.io/)
* [Facette on GitHub](https://github.com/facette/facette)
