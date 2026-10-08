# Starship Deployment Status

Starship Deployment Status is a small command-line client used by operators to
check the active control-plane environment before a release.

## Configuration

Hosted deployments use the Starship Cloud control-plane service. Private and
on-premises deployments may use operator-managed services instead. The client
does not hardcode a regional endpoint, so operators receive the appropriate
endpoint with their deployment configuration.

Copy `starship.ini.example` to `starship.ini` and set the service endpoint
provided by the deployment operator. Set `STARSHIP_API_KEY`, then run:

```bash
python3 app.py
```

The client authenticates to the configured service and prints its deployment
summary.

## Development

```bash
python3 -m unittest discover -s tests
```

## License

MIT
