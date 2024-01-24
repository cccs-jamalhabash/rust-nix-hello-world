# rust-nix-hello-world

```
cargo init
```

Add your flake.nix file. The one in this repo is a good start, it enables dev shell, binary build and docker image build. 

Use ```nix develop``` for dev shell.
Use ```nix build``` to build the binary.
Use ```nix build .#dockerImage``` to build the docker image. (docker image is from:scratch and contains the binary).

For nix build to work, you do need to generate the cargo.lock for your project. You can do that with ```cargo generate-lockfile```