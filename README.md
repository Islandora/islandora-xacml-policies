# Islandora XACML policies

Before installing Islandora the XACML policies located here should be copied into the Fedora global XACML policies folder. This will allow "authenticated users" in Drupal to access Fedora API-M functions. It is to be noted that the `permit-upload-to-anonymous-user.xml` and `permit-apim-to-anonymous-user.xml` files do not need to be present unless requirements for anonymous ingesting are present.

You will also have to remove some default policies if you want full functionality as well.

Remove deny-purge-datastream-if-active-or-inactive.xml to allow for purging of datastream versions.

More detailed information can be found in the 'Set XACML Policies' in the [Installing Fedora](https://wiki.duraspace.org/display/ISLANDORA713/Installing+Fedora) chapter of the documentation.
