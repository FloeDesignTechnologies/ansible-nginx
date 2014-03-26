nginx
========

Install (but don't configure) nginx on Debian based system.

Role Variables
--------------

- **nginx_apt_repository**: The source string for nginx APT repository to use.
- **nginx_apt_key**: The URL of the APT key for the nginx repository.
- **nginx_apt_packages**: The list of APT package to install for nginx, defaults
  to ```['nginx']```.

Example usage
-------------

    - role: nginx
      nginx_apt_repository: ppa:nginx/stable

    - role: nginx
      nginx_apt_repository: deb http://nginx.org/packages/debian/ wheezy nginx
      nginx_apt_key: http://nginx.org/keys/nginx_signing.key

License
-------

TODO
----

- Add support for more platforms.
- Add support for building from sources.

Apache v2

Author Information
------------------

Pierre Buyle <buyle@pheromone.ca>
