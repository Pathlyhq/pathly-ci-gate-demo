# Pathly CI gate demo

A pull request that breaks the user path turns the build red.

1. Record a Flow on [pathlyhq.com/try-flow](https://pathlyhq.com/try-flow) and keep it.
2. Create an API token in Pathly (Settings → Tech → Integrations) and add it as the repository secret `PATHLY_API_TOKEN`.
3. Add the Flow id as the repository variable `PATHLY_FLOW_ID`.
4. Push: the `Pathly gate` job runs the Flow and fails if it is not `ok`.

Pathly watches the path. Ping if it's up. Flow if a user can walk it. Chain if the services behind it hold.
