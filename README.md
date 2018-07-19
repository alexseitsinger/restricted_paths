# Restricted Paths Middleware

## Description

Limit access to specific urls based on environment, session session status, and account level.

## Installation

```python
pip install restricted_paths
```

## Usage

in settings.py:

```python
IS_DEVELOPMENT = DEBUG

RESTRICTED_PATHS = (
    "/admin",
)

MIDDLEWARE = (
    ...
    "restricted_paths.middleware.RestrictedPathsMiddleware"
    ...
)
```