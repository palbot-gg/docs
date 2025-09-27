# Kits

Palbot supports a **Kits** system that lets you define bundles of commands you can quickly give to players. This is useful for server rewards, events, or quick setup of player inventories.

---

## Available Commands

| Command | Description |
|---------|-------------|
| `/kits manage <optional existing kit>` | Create a new kit or modify an existing one. |
| `/kits delete <kit_name>` | Delete an existing kit. |
| `/kits give <userid> <kit_name> <server>` | Give a kit to a player on your server. |

---

## Kits Modal

When you run `/kits manage`, you’ll be presented with a modal to configure your kit. The fields are:

- **Kit Name**  
  The identifier for your kit. This name will show up in autocomplete when giving it to a player.

- **Commands (JSON)**  
  A JSON array of commands to run when the kit is given. Each command can include giving Pals, items, or experience.  
  > Tip: Use `{userid}` as a placeholder for the target player’s ID.

- **Description**  
  A human-readable description of your kit.

---

## Example Kits

### Multiple Items
Give a player a variety of items at once:

```json
["giveitems {userid} SFArmorWeight_5:1 Shield_SF:1 GYM_Head_Viking:1 AssaultRifleBullet:300 AssaultRifle_Default5:1 BLT:20 PalSphere_Exotic:100"]
```
Grant 10,000 XP, 5 berries, and a level 10 Anubis:

### Experience, Items, and a Pal

```json
["give_exp {userid} 10000", "give {userid} Berries 5", "givepal {userid} Anubis 10"]
```

---

## Best Practices
- Keep kit names short and descriptive.
- Use the description field to explain what the kit contains.
- Test your kits to make sure they're working correctly.
- Combine related items into one `/kits give` command when possible for less RCON requests to server.