# php-example

Simple php code for s2i build process on OpenShift mainly for demos and tests.


## Deploy php-example on OpenShift
Create a new project and the application resources:

```
oc new-project demo-php
oc new-app php~https://github.com/amigliet/php-example.git
```

Expose the application via an OpenShift route:

```
oc expose svc/php-example
```

