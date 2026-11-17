# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Rust binary crate `leviathan-test` (edition 2021), currently a minimal skeleton: `Cargo.toml` and `src/main.rs`. No dependencies yet.

## Commands

- Build: `cargo build`
- Run: `cargo run`
- Test: `cargo test` (single test: `cargo test <test_name>`)
- Lint / format: `cargo clippy` / `cargo fmt`

Note: the Rust toolchain was not installed on the machine when the project was created (install via rustup).

## Conventions

- Commit messages are written in French (e.g. "Ajout du fichier README.md").
