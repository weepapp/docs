# Obtaining a token

If you want to obtain your user account token, open your [user settings](https://weep.ga/settings)
and go to the Developer tab.

Now you will see your token, it looks like the following:

```
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MTIzfQ.XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
```

!> <!-- Token warning -->
**Never share your token with anyone, even people you trust. When someone has your token
they can access all of your account data and send messages as you.**

<!-- End token warning -->

## The token

The first part (`eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9`) contains information about the token
like the type and the algorithm. In this case it's the following:

```json
{
  "alg": "HS256",
  "typ": "JWT"
}
```

The second part (`eyJpZCI6MTIzfQ`) contains information about your user account. In this case
it is the following:

```json
{
  "id": 123
}
```

The third part contains the hash of the private key and the signature of the token, in this
case it is censored.

## Scammers

Scammers may try to get your token, please remember that **we will never ask you for your token.**
Please report these scammers immedeatly via the [report form](https://weep.ga/report?form=scammer)
