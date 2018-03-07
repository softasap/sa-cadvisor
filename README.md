sa-cadvisor
===========

[![Build Status](https://travis-ci.org/softasap/sa-cadvisor.svg?branch=master)](https://travis-ci.org/softasap/sa-cadvisor)

cAdvisor (Container Advisor) provides container users an understanding of the resource usage and performance characteristics of their running containers. 
It is a running daemon that collects, aggregates, processes, and exports information about running containers. 
Specifically, for each container it keeps resource isolation parameters, historical resource usage, histograms of complete historical resource usage and network statistics. 
This data is exported by container and machine-wide.

cAdvisor has native support for Docker containers and should support just about any other container type out of the box. 
Strives for support across the board so feel free to open an issue if that is not the case. 
cAdvisor's container abstraction is based on lmctfy's so containers are inherently nested hierarchically.

Example of usage (all parameters are optional)

Simple

```YAML
  roles:
    - {
        role: "sa-cadvisor",
        cadvisor_version: "0.27.4",
      }
```

Advanced:

```YAML
  roles:
    - {
        role: "sa-cadvisor",
        cadvisor_version: "0.27.4",
        cadvisor_port: 9280, # to expose WEBUI
        cadvisor_install_dir: "/opt/cadvisor"
      }
```

Copyright and license
---------------------

Code is dual licensed under the [BSD 3 clause] (https://opensource.org/licenses/BSD-3-Clause) and the [MIT License] (http://opensource.org/licenses/MIT). Choose the one that suits you best.

Reach us:

Subscribe for roles updates at [FB] (https://www.facebook.com/SoftAsap/)

Join gitter discussion channel at [Gitter](https://gitter.im/softasap)

Discover other roles at  http://www.softasap.com/roles/registry_generated.html

visit our blog at http://www.softasap.com/blog/archive.html
