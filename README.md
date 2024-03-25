# Docker

### Pain points in the software development
  - **Environment Consistency:** ensuring consistency across different `runtime environments`, `development`, `testing`, and `production`. Developers often faced the problem of "it works on my machine" due to differences in the runtime environments.
  - **Dependency Management:** Managing `dependencies`, `libraries`, and `runtime environments` for different applications and projects was complex. It often required manual setup and configuration, leading to potential conflicts and compatibility issues.
  - **Isolation and Security:** Ensuring `isolation` and security of applications was challenging. Traditional methods relied on heavyweight `virtual machines`, which added overhead and complexity.

### Docker use case
![docker-usecase drawio (3)](https://github.com/Liu-Chen-CS/docker/assets/158779475/cd706366-15b0-49ed-be5e-86dfcd3549d9)


### Virtual Machine vs Docker
![Docker drawio](https://github.com/Liu-Chen-CS/docker/assets/158779475/003a0d90-602a-4063-ac93-147061c2abc5)

|       |  **Virtual Machine**  |  **Docker**  |
|-------|-------|-------|
|**How They Work**|It creates a `whole virtual computer` with its own `operating system` on a `physical server`|It runs applications in `isolated packages` that share the same operating system kernel of the `host machine`|
|**Resource Usage**|It's `heavier` because each VM needs its own operating system|It's `lighter` because containers share the host's operating system|
|**Speed**|`Slower` to start because it needs to boot up a whole operating system|`Starts quickly` because it doesn't need to boot up a separate OS|
|**Management**|`Requires more setup` and maintenance as each VM is like a separate computer|`Easier` to manage as containers are quick to deploy using pre-built images|
|**Isolation**|Provides `stronger isolation` as each VM has its own OS|Offers `lighter isolation` because they share the same OS kernel, but it's usually enough for most cases|

### Image & Container & Repository
  - **Image**: An image is like a `snapshot` or `template` of a software application. It contains all the necessary `files`, `libraries`, and `configurations` needed to run the application.
  - **Container**: A container is a runtime `instance` of an image. It's a `lightweight`, `isolated environment` that runs the software application based on the instructions provided by the image.
  - **Repository**: A repository is a storage location where `Docker images` are stored and managed. It can be either public or private.

### Docker Config
  - yum -y install yum-utils
  - yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
  - yum -y install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
  - docker -v


