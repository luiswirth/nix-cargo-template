# Nix Cargo Template

This is a template repository to get you started with creating a rust application using nix flakes.
The heart of this repository is the [`flake.nix`](./flake.nix) file, which sets rust using nix flakes up.

The flake uses the [`oxalica/rust-overlay`](https://github.com/oxalica/rust-overlay), which provides us with the different rust toolchain versions.
The toolchain we want to use, is specified in the [`rust-toolchain.toml`](./rust-toolchain.toml) file, which you can edit to your requirements.
The overlay then reads this toolchain file and gets the appropriate versions of the tools.

For this to work you need
- [Nix](https://nixos.org/) with [flakes](https://nixos.wiki/wiki/Flakes) enabled
- (optional) [direnv](https://direnv.net/)
- (optional) [direnv-nix](https://github.com/nix-community/nix-direnv)
