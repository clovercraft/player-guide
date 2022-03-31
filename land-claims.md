# Land Claims

Clovercraft uses the GriefPrevention plugin for managing player and admin land claims. Claims protect all of your items, containers, and animals inside them.

You'll create your first claim as soon as you place a chest in the world. This 9x9 claim exists as an early-game protection for new players. You can create more claims, resize them, remove claims, subdivide claims, and grant specific permissions to other players inside your claims.

## Essential Commands

| Command                   | Description                                                                     |
| ------------------------- | ------------------------------------------------------------------------------- |
| `/claimslist`             | List out all of your claims                                                     |
| `/trustlist`              | List permissions you've granted in a claim                                      |
| `/trust [name]`           | Grant a player full permissions inside a claim                                  |
| `/untrust [name]`         | Revoke a players permissions inside a claim                                     |
| `/containertrust [name]`  | Grant a player permissions to access chests and other containers inside a claim |
| `/accesstrust [name]`     | Grant a player permission to use buttons, levers, and beds inside a claim       |
| `/permissiontrust [name]` | Grants another player permission to control trust inside a claim                |
| `/trapped`                | Escape from a claim if you become trapped                                       |

## Claim Management

At any given time, you have a set number of blocks you can claim in the world. This starts at 2500, and increases gradually based on the time you've spent in game.

{% hint style="info" %}
Claim blocks do not accrue if you are AFK. You must actively be playing the game.
{% endhint %}

Most tasks related to managing your claims in-game involve the use of a golden shovel. When you are holding a golden shovel, you will receive a chat message that tells you how many claim blocks you have available. If you're standing inside a claim when you switch to the golden shovel, it will place some fake blocks at the corners and along the edges of the claim you are in.

{% hint style="info" %}
The glowstone, gold, wool, iron blocks, netherack, and redstone blocks used by the plugin to show you claim borders are not real and cannot be harvested. Breaking them will give you whatever block is actually in that position.
{% endhint %}

### Making a Claim

To set up a new claim, hold a golden shovel in your hand. Standing at one corner of the area you want to claim, right click on the ground. This will set the first corner of the claim. Then, walk to the opposite corner and right click on the ground again to set the other corner of the claim.

In order for the claim to take, the following conditions must be met:

* The player has enough claim blocks available to claim the requested area
* The new claim does not overlap with any existing claims (overlapped claims will be highlighted with redstone blocks and netherack)
* The player is in the overworld

Your new claim extends from where you created it all the way up to build limit. Your claim will also extend down into the ground below the starting position as you build below that point.

### Trusting Other Players

Once you've made a claim, no other players may place or break blocks, access containers, interact with animals, open gates, or press buttons / levers inside of your claim. You can grant trust to other players using the `/trust` commands.

{% hint style="warning" %}
Admins and Mods have the ability to ignore your claims and permission restrictions.
{% endhint %}

#### Access Trust

Access trust gives another player permission to open gates, toggle levers, and press buttons within your claim. You can grant this permission using the `/accesstrust [player]` command while standing inside of the claim.

#### Container Trust

Container trust gives another player all the permissions of Access Trust, in addition to the ability to open containers (such as chests). You can grant this permission using the `/containertrust [player]` command while standing inside of the claim.

#### Full Trust

Full trust gives another player all the permissions of Container Turst, as well as the ability to place and break blocks within your claim. You can grant this permission using the `/trust [player]` command while standing inside of the claim.

#### Permission Trust

Permission trust grants another player the ability to control trust inside of a claim, in addition to all of the permissions of full trust. We do not recommend that players use this in most cases. You can grant permission trust using the `/permissiontrust [player]` command while standing inside of the claim.

{% hint style="info" %}
Trust levels are inherited from highest to lowest. This means that if you grant someone container trust, they automatically get access trust. Similarly, granting full trust gives permissions for container and access trust.
{% endhint %}

{% hint style="info" %}
To grant a level of trust to anyone for a given claim, use the keyword "public" instead of a player name with any of the above commands.

You can grant trust on ALL of your claims by using the above commands while standing outside of your claims.
{% endhint %}

### Subdividing Claims

If you'd like more fine-grained control over who you're trusting and where, you can subdivide your claims to create smaller areas within them with specific permissions.

To subdivide a claim, hold a golden shovel while standing inside of a claim you own. Then type the command `/subdivideclaims` to enter subdivision mode.

Once you're in subdivision mode, you can select the corners of the subdivision using the same method you used for placing the top level claim. Right click on the ground at the two opposing corners of your desired subdivision.

Subdivisions do not count against your total claim blocks, since the blocks they control have already been counted in your top level claim.

If you'd like to grant specific permissions inside of a subdivision, you can use any of the trust commands while standing in that subdivision. The trust will extend only to the edges of that subdivision, not the entire top level claim.

{% hint style="warning" %}
Claims cannot be divided vertically.
{% endhint %}

### Removing Claims

To remove any claim that you own, you can use the `/abandonclaim` command. This will remove the claim you are currently standing in. If you want to remove a subdivision, **and** the top-level claim it is a part of, use the `/abandontoplevelclaim` command.

You can also remove all of your claims at once if you plan on starting the claim process over by using the `/abandonallclaims` command.

## Claims and World Behavior

Claims have some odd impacts on the behavior of some parts of the world. Here are a few notable details to pay attention to

* Water cannot flow past the edge of a claim
* Lava cannot flow past the edge of a claim
* Pistons will not push blocks outside of a claim
