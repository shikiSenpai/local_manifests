

### Sync ###

```bash
# Initialize local repository
repo init -u https://github.com/shikiSenpai/local_manifests -b main


# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

```

### Build ###

```bash

# Set up environment
. build/envsetup.sh

# Choose a target
lunch evolution_$DEVICE-userdebug

# Build the code
m evolution
```
