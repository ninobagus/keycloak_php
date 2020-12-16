###setup

keycloak.json holds config

add backendconfig.json according to example

for this example I set up keycloack 2.4.0 and:
* started keycloak server with `./bin/standalone.sh -Djboss.socket.binding.port-offset=100`
* created realm "testRealm"
* created client "keycloaktest"
* created some user

to imitate an introspection on the received token by some other php application I
* created client "testBackend" using Basic authorization
