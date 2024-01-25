# monk-chroma

This repository contains Monk.io template to deploy openGPTs (https://github.com/chroma-core/chroma).

## Prerequisites

- Install Monk
- Register and Login Monk
- Add Cloud Provider


## Clone Repository

```bash
git clone https://github.com/monk-io/monk-chroma
```

## Load Template

```bash
cd monk-chroma
monk load MANIFEST
```


## Deploy

```bash
monk run chroma/chroma               
? Select tag to run [local/chroma/chroma] on: local
✔ Starting the run job: local/chroma/chroma... DONE
✔ Preparing nodes DONE
✔ Checking/pulling images...
✔ [================================================] 100% ghcr.io/chroma-core/chroma:latest local
✔ Checking/pulling images DONE
✔ Starting containers DONE
✔ Runnable templates/local/chroma/chroma connections graph updating DONE
✔ Runnable templates/local/chroma/chroma services initialization DONE
✔ Runnable templates/local/chroma/chroma connections graph has been updated DONE
✔ Runnable templates/local/chroma/chroma services have been initialized DONE
✔ Host ports have been added to container a4ccc73f8c12827a063b6e4baebeceb4-al-chroma-chroma-chroma DONE
✔ New container a4ccc73f8c12827a063b6e4baebeceb4-al-chroma-chroma-chroma created DONE
✔ Container a4ccc73f8c12827a063b6e4baebeceb4-al-chroma-chroma-chroma has been started DONE
✔ Started local/chroma/chroma
🔩 templates/local/chroma/chroma
 └─🧊 Peer local
    └─🔩 templates/local/chroma/chroma 
       └─📦 a4ccc73f8c12827a063b6e4baebeceb4-al-chroma-chroma-chroma running
          ├─🧩 ghcr.io/chroma-core/chroma:latest                 
          ├─💾 /Users/alexneleipa/.monk/volumes/chroma -> /chroma/chroma
          └─🔌 open (public) 176.104.61.186:5432 -> 5432

💡 You can inspect and manage your above stack with these commands:
        monk logs (-f) local/chroma/chroma - Inspect logs
        monk shell     local/chroma/chroma - Connect to the container's shell
        monk do        local/chroma/chroma/action_name - Run defined action (if exists)
💡 Check monk help for more!
```