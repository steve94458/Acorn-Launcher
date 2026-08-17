# Acorn Launcher

An open-source launcher for Minecraft: Java Edition, written in Python.

## About

Ember is a personal, non-commercial hobby project. It handles the parts of
running Minecraft that the official launcher makes awkward: keeping separate
instances for different versions and mod sets, installing mod loaders without
manual setup, and applying performance mod presets in one step.

## Features

- Downloads and installs any released Minecraft version
- Isolated instances — each with its own mods, configs, and saves
- Fabric mod loader installation
- One-click performance presets (Sodium, Lithium, Iris)
- Configurable JVM arguments and memory allocation
- Sign in with a Microsoft account

## Authentication

Ember uses the standard Microsoft OAuth 2.0 authorization code flow with PKCE.

Users sign in through the official Microsoft login page opened in their own
browser. **The launcher never sees, handles, or stores account credentials.**
Only the refresh token is retained, and it is stored in the operating system's
credential store (Windows Credential Manager / GNOME Keyring) rather than in a
plaintext file.

Ember does not bypass authentication, does not support cracked accounts for
online play, and does not modify any Minecraft functionality.

## Status

Under active development. Not yet released.

## Tech stack

Python 3.13 · requests · keyring · minecraft-launcher-lib

## Disclaimer

Not an official Minecraft product. Not approved by or associated with Mojang
or Microsoft.
