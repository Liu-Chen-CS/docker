# Docker

### Virtual Machine vs Docker
|       |  Virtual Machine  |  Docker  |
|-------|-------|-------|
|How They Work|It creates a `whole virtual computer` with its own `operating system` on a `physical server`|It runs applications in `isolated packages` that share the same operating system kernel of the `host machine`|
|Resource Usage|It's `heavier` because each VM needs its own operating system|It's `lighter` because containers share the host's operating system|
|Speed|`Slower` to start because it needs to boot up a whole operating system|`Starts quickly` because it doesn't need to boot up a separate OS|
|Management|`Requires more setup` and maintenance as each VM is like a separate computer|`Easier` to manage as containers are quick to deploy using pre-built images|
|Isolation|Provides `stronger isolation` as each VM has its own OS|Offers `lighter isolation` because they share the same OS kernel, but it's usually enough for most cases|
