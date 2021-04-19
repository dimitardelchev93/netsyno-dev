# netsyno-dev
Makes development a bit easier

## Steps to start

Add the `inopai-dev.project-path` setting for your vs code

## Commands
```
{
  run-local-frontend: "Run localhost:9000 frontend",
  run-beta-frontend: "Run beta.inopai.com frontend",
  run-stihl-frontend: "Run dev.service.stihl.inopai.com frontend",
  run-schnelltest-frontend: "Run dev.schnelltest.inopai.com frontend",
  run-local-elastic: "Run local inopai elastic search",
  fix-local-elastic: "Fix local inopai elastic search",
  run-local-honcho: "Run local honcho server",
  migrate-local-backend: "Migrate local backend",
  stop-all-running: "Stop all funcitonalities",
}
```

## Tasksets
```
{
  run-locally: "run-local-elastic,migrate-local-backend>run-local-honcho,run-local-frontend",
}
```

## Settings
```
{
  inopai-dev.project-path: "~/projects/inopai", // path to inopai project folder (REQUIRED),
  inopai-dev.autostart: "run-locally", // zero for no autostart or taskset id (default: 0),
}
```

### Release Notes
#### 1.0.0
Initial release of inopai-dev
