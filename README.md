# DeadlyISwitch's instant Swapper

Quick switch between the four powers in inFAMOUS Second Son for the PC port (HayatoG/iss_pc, CUSA00223).

link : https://github.com/HayatoG/iss_pc

Each power keeps its own bar and its own missiles. The shortcut only works if that save already has it recorded.

## Installation

1. Copy `DeadlyISwitch's instant Swapper.xml` into the port folder, inside `user\mods`.
2. Quit the game completely and open it again from the launcher.

The launcher applies the mod on startup. A change made mid-session does not take effect until the next launch. The game creates `user\poderes.bin` on its own, in the `user` folder next to the launcher. The name of that folder does not matter.

You do not need `patches.bin`, `mods.json`, or any Python program.

## Controls

Keyboard:

- 4 smoke
- 5 neon
- 6 video
- 7 concrete

Controller. Hold the top face button (triangle, Y, or the Switch X) and press:

- right stick: smoke
- D-pad left: neon
- D-pad right: video
- D-pad up: concrete

Down does nothing. It works the same on PlayStation, Xbox, and Switch controllers.

## How shortcuts get recorded

At the start, there are no shortcuts. Not even smoke.

A power gets recorded when its bar goes up or down while you are using it. Absorbing it is the usual way. Spending it counts too.

If the recorded power is further along, the earlier ones get recorded as well. The order is smoke, neon, video, concrete.

- Neon also records smoke.
- Video also records neon and smoke.
- Concrete also records video, neon, and smoke.

In a late-game save, absorbing the highest power you already have is enough. You do not have to go through them one by one. The shortcut does not appear just because you have the power in the story: that power's bar has to move at least once with the mod installed.

## Bar and missiles

Energy you recharge stays on that power. Switching from smoke to neon leaves the neon bar where it was, and when you come back smoke is still as you left it.

Each power has its own missile reserve. Spending one does not spend the others.

## One record per save

`user\poderes.bin` stores one record for each slot in the load menu: User0 through User9, and the two autosave slots. That is where the bar, the missiles, and the shortcuts for that save go.

You have to load the save from the load menu. The first time this mod sees a slot, that record starts with no shortcuts and does not inherit the ones from the previous save. As you use it, only that slot gets recorded. If you load it again, what was already recorded comes back, including after you close the game.

Continue, without going through that menu, keeps the record that was already open.

That file is each person's progress. It is not shared.

## How to say thanks?

Just give me a star on GitHub and we're good!
