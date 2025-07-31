# Agent Instructions for `prompts-nvim`

This document provides guidance for LLM agents working on the `prompts-nvim` repository.

## Project Overview

This repository contains the Neovim plugin for the Prompts project. It is a Lua-based plugin that interacts with the `prompts-cli` binary using RPC.

## Core Tenets

- **Dependabot is Authoritative:** The `prompts-cli` binary is a dependency that is managed by Dependabot. Do not manually update this dependency.
- **Focus on the Vim Experience:** The primary focus of this repository is the user experience within Neovim. The core logic is handled by the `prompts-cli` binary.
- **Asynchronous Operations:** All interactions with the `prompts-cli` binary must be asynchronous to avoid blocking the Neovim UI.

## Development Workflow

1.  **Understand the `prompts-cli` RPC API:** Before making any changes, familiarize yourself with the RPC API of the `prompts-cli` binary.
2.  **Write Unit Tests:** For any new Lua code, write a unit test using the `busted` testing framework.
3.  **Write Integration Tests:** For any new feature that interacts with the `prompts-cli` binary, write an integration test that runs the plugin in a headless Neovim instance.
4.  **Run All Tests:** Ensure that all tests, including unit and integration tests, pass.

## Key Commands

- **Run tests:** `make test`
