Role Apache2
=================

Install and configure packages that must be on all netensia's web servers
It installs apache2 and deploys vhosts 

Role Variables
--------------

| Name                     | Default       | Description                                                         |
|--------------------------|---------------|---------------------------------------------------------------------|
| has_ssl                  | False         | set True for https server                                           |
| ssl_folders              | ../files      | folder where are ssl certs and keys                                 |
| ssl_certs                | default([])   | certificate file for SSL encryption                                 |
| ssl_keys                 | default([])   | private key file for SSL encryption                                 |
| vhosts                   | default([])   | dictionnary ( srv=> ,name=> ) that list informations of vhost files |
| docroot                  | /var/www      | default doc root                                                    |
| default_site             | 000-default   | vhost that must be deleted                                          |
| simple_site              | True          | This add a default simple site based on ansible_fqdn                |
|--------------------------|---------------|---------------------------------------------------------------------|


