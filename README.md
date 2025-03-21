# Getting Started

Welcome to your new project.

It contains these folders and files, following our recommended project layout:

File or Folder | Purpose
---------|----------
`app/` | content for UI frontends goes here
`db/` | your domain models and data go here
`srv/` | your service models and code go here
`package.json` | project metadata and configuration
`readme.md` | this getting started guide


## Next Steps

- Open a new terminal and run `cds watch`
- (in VS Code simply choose _**Terminal** > Run Task > cds watch_)
- Start adding content, for example, a [db/schema.cds](db/schema.cds).

## Podman commands

For this training we're using Podman instead of Docker, so here are the commands for the solution:

- `podman build -f ./Dockerfile --tag demo:latest`
- `podman images`
- `podman container run -it --rm -p 4004:4004 -d --name DemoContainer localhost/demo:latest`
- `podman container ls`
- `podman stop DemoContainer`
- `podman image rm localhost/demo`

Attaching to the running session can be done with:

```
podman attach DemoContainer
```

Detaching can be done using the default CTRL+P,CTRL+Q combination.

## Learn More

Learn more at https://cap.cloud.sap/docs/get-started/.
