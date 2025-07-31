# TODO for `prompts-nvim`

This document outlines the implementation plan for the `prompts-nvim` project, based on the requirements in the PRD.

## Phase 1: Basic Plugin Structure

- **Task 1: Initialize the Neovim plugin**
    - Sub-task: Set up the basic plugin structure.
    - Sub-task: Define basic commands and keybindings.
    - Test: Write unit tests for basic plugin loading and command execution.

- **Task 2: Implement RPC communication with `prompts-cli`**
    - Sub-task: Establish asynchronous communication with the `prompts-cli` binary.
    - Sub-task: Define the RPC schema for prompt management operations.
    - Test: Write integration tests for RPC communication.

## Phase 2: Core Functionality

- **Task 3: Implement prompt listing**
    - Sub-task: Call `prompts-cli` to list all prompts.
    - Sub-task: Display prompts in a Neovim buffer.
    - Test: Write E2E tests for listing prompts.

- **Task 4: Implement prompt viewing**
    - Sub-task: Open a selected prompt in a new buffer.
    - Test: Write E2E tests for viewing prompts.

- **Task 5: Implement prompt editing**
    - Sub-task: Allow editing of prompt content in a buffer.
    - Sub-task: Save changes back to `prompts-cli`.
    - Test: Write E2E tests for editing and saving prompts.

## Phase 3: Enhanced Features

- **Task 6: Integrate with Telescope.nvim**
    - Sub-task: Implement fuzzy finding for prompts using Telescope.
    - Test: Write E2E tests for Telescope integration.

- **Task 7: Implement Lua API**
    - Sub-task: Expose core plugin functionality through a Lua API.
    - Test: Write unit tests for the Lua API.
