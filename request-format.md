# Request format

## The API namespace

The API namespace groupes the api under another subdirectory,
like the following: `https://weep.ga/api/{version}`

If a request is defined like the following: `GET /user`, then it always means that
the version is the latest version (currently v0) and the request path is the follwing:
`https://weep.ga/api/v0/user`

### Versions

The latest verion is `v0`. The following versions exist right now:

- `v0`

Only the latest version is documented and supported, older versions may not
work or lack functionality. Always use the latest version for the best results.

## Headers

You will need to set the following headers to access routes where auth is required:

```yaml
Authorization: Bearer <token>
```

Find out how to obtain a token [here](obtain-token.md)
