# Palbot Setup Guide

## What is Palbot?
Palbot connects to your Palworld dedicated server using RESTAPI to execute remote commands and gather information. It can also utilize RCON if enabled.

---

## 1. Enable REST API
To allow Palbot to communicate with your server, RESTAPI must be enabled.

1. In the same `PalWorldSettings.ini` file, ensure this section is enabled:
```
AdminPassword="YourPassword",RESTAPIEnabled=True,RESTAPIPort=8212
```
- **RESTAPIEnabled**: Must be set to `True`.
- **RESTAPIPort**: Default is `8212`.

---

## 2. Enable RCON (Optional)
RCON Port is required for the `/palcon` command.

1. Open your `PalWorldSettings.ini` file.
2. Make sure the following settings are present and configured:
```
AdminPassword="YourPassword",RCONEnabled=True,RCONPort=25575
```
- **AdminPassword**: Set a strong admin password.
- **RCONEnabled**: Must be set to `True`.
- **RCONPort**: Set the port; default is usually `25575`.

---

## 3. Add Your Server to Palbot

Use the `/addserver` command in Discord and fill out the following fields:

- **Server Name**: A unique name for your server (can be anything).
- **Host**: The address used to connect (example: `127.0.0.1`).
- **REST API Port**: The port used for the REST API (if enabled).
- **RCON Port**: The port you configured for RCON. (optional)
- **Password**: The RCON admin password.

---

## 4. Test Your Setup

- Use `/serverinfo` to test REST API connectivity.

If both return results, your setup is complete!
