# Gemini Development Guide: Prompts Neovim

This document guides the development of the Prompts Neovim plugin.

## Project Overview

The Prompts Neovim plugin is a Lua-based plugin that provides an interface to the `prompts-cli` binary. It allows users to manage their prompts from within Neovim.

## Core Tenets

- **Lua for Neovim:** The plugin will be written in Lua to ensure seamless integration with Neovim.
- **Asynchronous Operations:** All interactions with the `prompts-cli` binary will be asynchronous to avoid blocking the Neovim UI.
- **Vim-style Keybindings:** The plugin will use Vim-style keybindings for all interactions.

## Development Workflow

1.  **Test First:** For any new feature, write a failing test that clearly defines the desired behavior.
2.  **Implement:** Write the minimum amount of code required to make the test pass.
3.  **Refactor:** Refactor the code to improve its design, readability, and performance, ensuring all tests still pass.
4.  **Repeat:** Repeat the cycle for the next feature.

## Key Technologies

- **Lua:** The primary programming language.
- **Neovim RPC:** For communication with the `prompts-cli` binary.
- **Telescope.nvim:** For fuzzy finding prompts.

## Initial Setup

1.  **Initialize Plugin Structure:** Set up the basic directory structure for a Neovim plugin.
2.  **Write First Test:** Write a simple test to ensure that the basic plugin loading is working correctly.
