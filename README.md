# rp2040-zero-rs-template
A quick Rust template repo for the RP2040-Zero microcontroller board

This template is based on the following example: https://github.com/rp-rs/rp-hal-boards/tree/main/boards/waveshare-rp2040-zero

## Getting Started

To flash the contents of the repo onto an RP2040-Zero:

1. Install `cargo`.
2. Add target instruction set: `rustup target add thumbv6m-none-eabi`
3. Install tools for flashing:
```sh
# Useful to creating UF2 images for the RP2040 USB Bootloader
cargo install --locked elf2uf2-rs
# Useful for flashing over the SWD pins using a supported JTAG probe
cargo install --locked probe-rs-tools
```
4. Plug in the RP2040, then run `cargo run`.
