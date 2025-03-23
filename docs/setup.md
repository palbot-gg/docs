# Palbot Setup Guide

## What is Palbot?
Palbot connects to your Palworld dedicated server using RCON to execute remote commands and gather information. It can also utilize the REST API if enabled.

---

## 1. Enable RCON
To allow Palbot to communicate with your server, RCON must be enabled.

1. Open your `PalWorldSettings.ini` file.
2. Make sure the following settings are present and configured:
```
AdminPassword="YourPassword",RCONEnabled=True,RCONPort=25575
```
- **AdminPassword**: Set a strong admin password.
- **RCONEnabled**: Must be set to `True`.
- **RCONPort**: Set the port; default is usually `25575`.

---

## 2. Enable REST API (Optional)
The REST API is required for commands like `/serverinfo` and `/livemap`.

1. In the same `PalWorldSettings.ini` file, ensure this section is enabled:
```
AdminPassword="YourPassword",RESTAPIEnabled=True,RESTAPIPort=8212
```
- **RESTAPIEnabled**: Must be set to `True`.
- **RESTAPIPort**: Default is `8212`.

---

## 3. Add Your Server to Palbot

Use the `/addserver` command in Discord and fill out the following fields:

- **Server Name**: A unique name for your server (can be anything).
- **Host**: The address used to connect (example: `127.0.0.1`).
- **RCON Port**: The port you configured for RCON.
- **Password**: The RCON admin password.
- **REST API Port**: The port used for the REST API (if enabled).

---

## 4. Test Your Setup

- Use `/rcon info` to test RCON connectivity.
- Use `/serverinfo` to test REST API functionality.

If both return results, your setup is complete!
