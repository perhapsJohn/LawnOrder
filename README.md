# Lawn Order (web build)

The browser build of **Lawn Order**, a voxel stealth game about a small dog with
a big grudge: sneak into the neighbours' yards, review every lawn on the list,
and slip out before anyone catches you. Or play the humans and catch the dogs.
Campaign, Arcade modes and online rooms (up to four players) through the
Wayside relay. Served by GitHub Pages at https://perhapsjohn.github.io/LawnOrder/
and played in the Scareathon arcade.

One page, two packs: phones and tablets load `index.mobile.pck` (touch controls,
a 1280 x 720 layout, no desktop-only music layers); desktops load `index.pck`.
`?pack=mobile|desktop` forces one.

Inside the Scareathon arcade it asks for the arcade session (`unityReady`) to
use the signed-in username, and a finished Paper Route posts
`{type: "PLAYER_DIED", score}` (the route's total) to the page around it.

This repo holds only the exported files (Godot 4.6 web export); the game's
source lives elsewhere and publishes here with `tools/export_web.py`.
