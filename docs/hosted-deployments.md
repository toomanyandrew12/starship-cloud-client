# Hosted deployments

Starship Cloud hosts the control-plane status service for managed deployments.
The client authenticates to the deployment's assigned regional endpoint with
the API key issued during provisioning. Endpoint values are distributed with
deployment configuration rather than embedded in the client source.
