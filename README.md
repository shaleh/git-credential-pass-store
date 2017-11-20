A simple git credential helper backed by [`pass`](https://www.passwordstore.org/).

Put the helper in your path and then run:

    git config credential.helper pass-store

or if you store your entries as "github.com" instead of "github":

    git config credential.helper "pass-store --full-host"

Now when git needs account info it will query `pass`. This only works
if your entries look like this:

    some-secret-sssh
    Username: user
