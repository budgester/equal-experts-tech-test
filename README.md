This will install a basic Jenkins CI/CD Server using ansible and ansible galaxy

Start the vagrant box.

```vagrant up```

Once the ansible has completed you can access Jenkins on the following url

http://localhost:8080


Username: admin
Password: admin


# Feedback

## Good Things:

Use of ansible plugin

Use of ansible galaxy to install roles

## Not so good things:

Documentation is not very good, no instructions apart from vagrant up. A good readme would include system requirements, software versions if used any, run and cleanup and troubleshooting instructions.

Use of community built jenkins role but there is no mention neither of the author or justification why this specific role was used in the first place.

Java is installed using a community role from same author, there is no version pinned and could break if author update java role without updating jenkins role.

Jenkins version is not pinned either.

Defaults have been used for security and there is no attempt made to address how to make login secure.
