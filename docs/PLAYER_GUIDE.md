# Simlas Player Guide

Simlas helps your table run characters, turns, and combat in Discord while C.O.D.I. remains the source for calculated character values. Use `/help` whenever you want the live command list or option details.

## Contents

- [Getting started](#getting-started)
- [Joining and choosing a character](#joining-and-choosing-a-character)
- [Rolls and resources](#rolls-and-resources)
- [Weapons and carried equipment](#weapons-and-carried-equipment)
- [Encounters and your turn](#encounters-and-your-turn)
- [Drawing and readying weapons](#drawing-and-readying-weapons)
- [Attacking, defending, and damage](#attacking-defending-and-damage)
- [Conditions and Critical Wounds](#conditions-and-critical-wounds)
- [Grapple, Pin, and Choke](#grapple-pin-and-choke)
- [Ambushes](#ambushes)
- [Status and troubleshooting](#status-and-troubleshooting)
- [Legacy C.O.D.I. migration](#legacy-codi-migration)

## Getting started

You need Discord access, a C.O.D.I. character sheet, and the join code from your GM. `/help` gives a private, current command guide without cluttering the game channel.

## Joining and choosing a character

Join with `/game join`, link your sheet with `/character link`, and bring it into the game with `/game bring`. Use `/game use` if you need to change your active brought character. `/character show` and `/game characters` are useful checks before play.

Keep the sheet shared with Simlas's Google service account. If a value cannot be read, ask the GM for sharing help rather than repeatedly retrying a command.

## Rolls and resources

Use `/roll` for ordinary skill, profession, and STAT checks outside a turn. Choose the check from autocomplete and add Luck, a situational modifier, DC, task, or comment only when appropriate. Skill totals must beat the DC; STAT checks use their own roll-under presentation.

Use `/turn roll` when a check is your Action in combat. `extra:true` uses an Extra Action when legal. `/vitals status` shows current resources.

## Weapons and carried equipment

`/weapons list` shows weapon slots. `/weapons equip` and `/weapons unequip` change whether a weapon is carried. Carrying a weapon is not the same as drawing it during an encounter.

## Encounters and your turn

Use `/encounter status`, `/encounter participants`, and `/encounter initiative status` to orient yourself. Roll when asked with `/encounter initiative roll`.

`/turn status` shows your available actions and drawn weapon. `/turn hold`, `/turn active-dodge`, `/turn recover`, `/turn action`, and `/turn done` support common turn choices.

## Drawing and readying weapons

Use `/turn draw` to draw a carried weapon. A normal draw consumes an Action; `extra:true` may use your Extra Action where legal. A one-handed weapon defaults to your functional Main hand; use the optional `hand:Off` only for an unusual draw. A two-handed weapon occupies Both hands. The weapon stays drawn in the encounter and appears in `/turn status`; it is also the item Simlas permits you to use for Block or Parry.

Put a shield in C.O.D.I.'s dedicated shield slot to identify the shield you carry, then use `/turn shield` to draw or stow it. A ready shield occupies your functional Off-hand; Off is not inherently Left or Right. Shield draw/stow uses the normal Action or an eligible Extra Action; asking for its current ready/stowed state is a no-op and costs nothing. A shield must be ready to Block; only a ready Manticore Shield may Parry. A ready shield may coexist with a one-handed weapon, but not a two-handed weapon. `/turn drop` immediately drops your currently held weapon or ready shield without consuming an Action; it remains on your C.O.D.I. sheet but is unavailable in this encounter. Your GM may enable a campaign option that combines a one-handed weapon draw with drawing the dedicated shield.

An Elf with Marksman may draw and string a bow without consuming that Action. To switch weapons, draw the other carried weapon first.

`/turn hand-switch` moves your currently held one-handed weapon between functional Main and Off when the destination is free. It is Simlas bookkeeping only: it costs no Action, STA, or Movement. If an item was dropped, `/turn pick-up` recovers the tracked weapon or shield when the GM permits the physical circumstance. Per Core p.151, **Pick Up/Draw an Item or Weapon** costs a Normal Action or eligible `extra:true` Extra Action; it does not duplicate C.O.D.I. inventory.

An active Dismembered Arm makes that physical arm unavailable for holding equipment. Simlas will reject a draw, shield, hand switch, preparation, or pickup that would use it; it will not silently choose your other hand.

## Attacking, defending, and damage

For a PC, `/attack source:` offers only the currently drawn weapon, **Punch**, and **Kick**. Other carried weapons are unavailable until you use `/turn draw`. NPC and bestiary combatants use their listed attacks.

The usual combat flow is:

```text
/attack
→ /defend
→ /damage resolve
```

Choose the offered target, form, range, and other options. Bows allow Single Strike or Strong Strike, never Fast Strike. Crossbows allow Single Strike only.

**Disarm** is a Normal-Action attack substitute. It uses your held melee weapon (or Brawling when unarmed), then normal defense. On success it drops the target's held weapon, rolls distance and Core p.163 Scatter for the GM to interpret, and deals no HP damage—there is no `/damage resolve` step. A dropped PC weapon is recovered with `/turn pick-up item:Weapon` when the GM permits it.

Ranged attacks require suitable range and ammunition selection. A committed shot consumes one projectile, including a miss; a declaration rejected before firing consumes none. A bow stays ready after firing. A crossbow becomes unloaded after its committed shot: use `/crossbow load` on a later legal Action before firing it again.

Silver-Coated ammunition is visibly labelled, for example `Silver Coating 1d6`. Select it normally; Simlas applies the campaign Silver rule and rolls its Silver damage when appropriate. Do not add those dice yourself.

Supported weapon and ammunition effects resolve from your C.O.D.I. values. Percentage effects follow the campaign's effect-roll setting; a 100% effect applies without a percentage roll. Experimental ammunition and unsupported effect text remain GM-handled.

Damage resolution applies supported damage, armor, Critical, wound, Stun, condition, and death/defeat results. If Simlas says damage was committed but could not render the receipt, do **not** resolve it again. Ask the GM to use the same Attack number with `/damage resolve` to show the stored result safely.

## Conditions and Critical Wounds

Use `/condition status` to see active conditions. Your GM manages condition changes and may ask you to make required rolls. Critical Wounds and their treatment use the `/critical` command family; follow the GM's instructions and inspect the current wound state when needed.

## Grapple, Pin, and Choke

Use `/special` for available special-combat actions and `/special defend` when prompted. Grapple, Pin, Choke, and Escape are turn-bound actions with their own legal responses; follow the prompt rather than reproducing a roll manually.

## Ambushes

During Ambush Setup, the GM records awareness. If you are an ambusher, choose your real opening attack through `/attack → /defend → /damage resolve`. Ambush happens before Initiative and does not replace your later combat choices.

## Status and troubleshooting

Useful checks include `/help`, `/turn status`, `/encounter status`, `/encounter participants`, `/condition status`, and `/vitals status`.

If a command looks wrong, stop before repeating it. Check your active character, the bound game channel, current turn, and sheet sharing; then give the GM the command and response you saw. Retry only when Simlas explicitly tells you to resume or retry the same action.

## Legacy C.O.D.I. migration

Older sheets can be migrated with the separate C.O.D.I. Migration Utility. It creates a current sheet without replacing the original. Ask your GM or administrator for the campaign procedure.
