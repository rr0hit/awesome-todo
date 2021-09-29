# Applications 

List of Applications intent for your catalog. This can be bunch of monoliths or microservices as per your design

There are three applications defined here.

1. A Backend Application
2. A Frontend Application
3. Rock Mongo to access mongo.

## Stack Details

### Backend Application

* spec.release.build: Fixed Image, with rolling release strategy
* runtime.ports: Works on port 3000
* runtime.healthcheck: Health check is defined as port check on 3000, if this port is open application is considered healthy
* runtime.autoscaling: Application can autoscale from 1 to 3 instances with 50% cpu as threshold
* runtime.size: Size of the pod
* permission: Accesses *demomongo* with Read write permission
* env: Static environment variables
* env.MONGODB_USER: Create a user in *demomongo* and communicate it to this environment variable

### Frontend Application

* loadbalancing.rules: route all request in domain defined by  *demoingress* on path starting with */* to 3000 port of this application.

