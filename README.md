# rust-nix-hello-world

Start your project with ```cargo init``` as usual.

Add your flake.nix file to the root of the project. The one in this repo is a good start, it enables dev shell, binary build and docker image build. 

Use ```nix develop``` for dev shell.
Use ```nix build``` to build the binary.
Use ```nix build .#dockerImage``` to build the docker image. (docker image is from:scratch and contains the binary).

For nix build to work, you do need to generate the cargo.lock and commit it to your repo. You can do that with ```cargo generate-lockfile``` and then commit with git.

## Resources
- https://zero-to-nix.com/
- https://fasterthanli.me/series/building-a-rust-service-with-nix/part-11#building-catscii-with-nix-build
