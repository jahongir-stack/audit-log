# audit-log

Append-only HMAC-SHA256 integrity audit log with a chain of tamper-evident events.

Python 3.11+; no third-party dependencies.

## Run tests

From the repository root:

```sh
python -m unittest discover -s . -p 'test_core.py' -v
```

## Contents

- `core.py`: implementation
- `test_core.py`: unit tests and usage examples
- `.github/workflows/tests.yml`: CI tests on Python 3.11–3.13

## Production limitations

The HMAC key must remain secret. This demo is in-memory and lacks durable storage and key rotation.

This is a learning/portfolio reference, not an audited production service.
