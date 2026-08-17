# What's new

Newest first. Written for the people using the app, not for the people building it.

---

## 2.13 — 17 August 2026 · test release

### Fixed
- **The dashcam recorded nothing.** It said "Recording", it created files, and every one of them
  was empty. Unlokit was asking the camera for a frame rate it does not offer, and asking in a way
  that meant the refusal was never reported — so it looked like it was working.
- **The dashcam now tells the truth about itself.** It says "Recording" only once pictures are
  actually arriving, "Starting…" until then, and "No picture from this camera" if none ever come.
- **Recordings show their real size.** Anything under half a megabyte used to read "0 MB", so a
  clip with a little in it and a clip with nothing in it looked the same. An empty one now says
  "empty — nothing recorded".
- A camera that produces no picture no longer leaves empty files behind, and is retried later
  instead of every few seconds.

## 2.12 — 17 August 2026 · test release

### What's new
- **Dashcam.** Settings › Vehicle › Dashcam records while you drive. Pick any of the four cameras
  that look at the road — front, rear, left mirror, right mirror — and record one or all four at
  once. Front only to start with.
- **It records the road, never the cabin.** The car also has cameras pointed at the driver and the
  passengers. Unlokit will not record those, and there is no setting that turns that on.
- Recordings are named by camera and time, kept in segments, and the oldest are deleted
  automatically once you reach the storage limit you set. Nothing is ever sent anywhere.
- **The car borrows a camera and gives it back.** Selecting reverse takes the rear camera and the
  360 view takes all four. The Dashcam screen says which camera the car has, and recording picks up
  again by itself.

### Careful
- **Still a test release.** The dashcam has never run in a car — this build is how it gets tried
  for the first time.
- Check the storage limit before a long drive. Four cameras fill space roughly four times as fast
  as one, and that limit is what stops it filling the disk.

---

## 2.11 — 16 August 2026 · test release

### What's new
- **Your car's hidden settings.** Settings › Vehicle › Car configuration opens 66 settings the car
  has but never shows you — drift mode, tank turn, camping levelling, the badge light, engine noise
  cancelling, the roof display and the rest. Search them, switch them, and put every one of them
  back with a single button.
- **Round widgets.** Any widget except the two navigation strips can be a dial instead of a card.
  Hold a tile on the home screen and pick **Shape**, or use **Shape** in the widget composer.
- The compass, g-force and moon dials were redrawn rather than shrunk. As a circle the compass
  needle moves out to the rim so the heading reads in the middle, and the moon becomes the whole
  widget.

### Careful
- **This is a test release**, offered only to cars with test releases turned on. None of it has
  been used in a car yet.
- **Car configuration writes to the car itself, not to Unlokit.** Those settings stay changed even
  if you uninstall this app. Unlokit writes down what each one was before touching it, so *Put
  everything back* restores exactly that — but the six that change how the car drives ask first,
  and they are worth leaving alone unless you know what they do.
- **A switch there may do nothing.** The values Unlokit sends are the ones the car's own settings
  app uses, but nobody has confirmed them on this model yet. If something turns on and will not
  turn off, hold the row and type the value by hand.

---

## 2.10 — 16 August 2026

### What's new
- **Tiles stay exactly where you put them.** The home screen no longer rearranges itself when you
  add or remove something.
- Removing a tile leaves the space empty instead of stretching the others to fill it. One tile left
  stays one tile, not a card covering the screen.
- **Add always works.** If the screen is full it takes half of the biggest tile, so you no longer
  have to go and resize something first.
- Preferred the old behaviour? **Home setup › Rearrange tiles automatically** turns it back on.

### Better
- The **Add tile** button is properly sized and labelled, and matches the DONE button beside it.

---

## 2.09 — 16 August 2026

### Fixed
- **Adding a tile no longer rearranges everything else.** Tiles you have already placed stay exactly
  where they are.
- A new tile lands in the first free space, top-left first — the same place every time, instead of
  somewhere different on each try.
- The first tile on an empty screen is a normal size now, not one card filling the whole area.

### What's new
- **Run an app here** is on the **+** menu, so you can add a tile that runs Spotify without
  converting an existing tile first. It starts large, because an app needs room to draw.
- The **+ Add** button is much bigger and easier to reach from the driver's seat.

---

## 2.08 — 16 August 2026

### Fixed
- **Removing home tiles works.** You can take off as many as you like, right down to none.
- The cause: removing the *last* tile quietly put all of them back. So nine removals looked fine and
  the tenth undid everything — which looked exactly like removal being broken.
- An empty home screen is a real choice now. It shows "Tap to add one", and holding it brings back
  everything you removed.

### What's new
- A tile running an app can be pointed at a different one with **Change the app**, without stopping
  it first.
- Removing a tile that was running an app also stops the app, instead of leaving it running
  somewhere you cannot see it.

---

## 2.07 — 16 August 2026

### What's new
- The "what's new" you are reading is laid out properly — headings, real bullets, no wall of text.
- If you have skipped a few versions, the update screen now shows what changed in those too, behind
  **See what else changed**.

### Better
- It tells you how many versions behind you are, so it is clear what you are catching up on.

---

## 2.06 — 15 August 2026

- **Run a real app inside a home tile.** Hold a card, choose **Run an app here**, and pick Spotify or
  YouTube Music — it actually runs there, playing and touchable. Not an icon that opens it: the app
  itself, in the tile.
- **One tile at a time.** Choosing a second tile moves it rather than adding another, because each
  running app costs real performance on top of the launcher and the cluster.
- **Try it on a big tile first.** A small tile gives the app very little room to draw.
- If system access is not available, the tile falls back to a card that opens the app the normal way.

---

## 2.05 — 15 August 2026

- **Another go at removing home tiles.** The setting that records a removed card was stored in a way
  this ROM does not keep reliably. It is stored differently now.
- **Pinning a tile** used the same storage, so that should be more reliable too.
- If a card still will not go, the message now tells you it **failed** instead of claiming it worked.
  Please send what it says — it names which part is at fault.

---

## 2.04 — 15 August 2026

- **Removing a home tile actually removes it.** Press and hold a card, choose Remove, and it goes.
  It used to say "Removed" and leave the card on screen.
- **Cabin, Now playing and app shortcuts follow the Background setting.** Setting one to None really
  does clear its card — those three were ignoring it entirely.
- Home setup still brings back anything you removed, if you change your mind.

---

## 2.03 — 15 August 2026

- **Fixes 2.02 not starting at all.** If you are on 2.02 and the launcher will not open, install this.
- The home screen could die before it drew anything, so nothing could launch it — including
  DisplayMirror. The only way out was restarting the head unit.
- Instrument screen and system access come back on their own once the app starts normally again.
- Everything from 2.02 is still here: full screen, clear widgets, readable settings.

---

## 2.02 — 15 August 2026

**The whole screen is yours.**
The car's status bar and navigation bar are hidden everywhere in the app, not just in split screen.
Swipe in from the top or bottom edge to bring them back for a moment; they tuck away again on their
own. If you would rather keep them — the clock lives up there — turn it off in **Appearance ›
Screen**.

**Widgets really do have no background now.**
The last version said they would and they did not: a background was being written onto every widget
the moment it was placed, so the new default never got a chance. Fixed, and existing widgets are
cleared too. Set one per widget from **Surface** if you want the card back.

**Glass you can read.**
Settings and the app drawer keep the frosted look, but the page behind them is darkened so the text
no longer changes contrast depending on what part of your wallpaper is underneath it. The search bar
and buttons in All Apps got the same treatment.

**Removing a home tile closes the gap.**
The tile went but the space it left stayed empty. The row now closes up.

**The background "Show it" switch works straight away** instead of needing you to leave the screen
and come back.

---

## 2.01 — 15 August 2026

**Settings are readable.**
The cards were letting the background photo show through behind the text, so how readable a setting
was depended on what happened to be behind it — dark writing over a bright part of your wallpaper,
light writing over a dark part, changing as you scrolled. The cards now stay solid enough to read
against, whatever background you have chosen and wherever the opacity slider is set.

**You can see the categories.**
The headings that group the settings were the smallest and faintest text on the screen. They are now
larger, brighter, and spaced so it is obvious which group each one belongs to.

**Signing in has real buttons.**
"Send me a code" and "Sign in" looked exactly like every other grey row, so there was nothing that
looked pressable on a screen with one thing to do. Both are proper buttons now, the email and code
boxes are labelled, and "Use a different email" is clearly the lesser of the two choices.

---

## 2.00 — 15 August 2026

**The tray updates as you press it.**
The fan number and the lit state of A/C, Defrost and daytime lights waited for the tray to be closed
and reopened before they caught up — the panel was being rebuilt a moment after each press and
asking the car again, and the car answers a beat late. Buttons now change immediately, then settle
to whatever the car reports.

**Split screen finds apps that wandered off.**
Coming back from the car's own settings could leave the panes empty while the app was still running
— YouTube kept playing, Maps kept its route, but neither was in the split. They were sitting on the
main screen, and the lookup that was supposed to find them only ever looked at freeform windows. It
now checks every running app and moves it back into its pane.

---

## 1.99 — 15 August 2026

**Widgets have no background by default.**
They used to arrive on a dark card whether it suited your wallpaper or not, and a screen of them
looked like a wall of boxes. Now they draw only themselves. If you want a card back, hold a tile on
the home screen and pick **Background** — Glass, Solid, Outline or None, per tile.

**Climate buttons respond to every press.**
Tapping fan **+** three times moved it one step, and the number only caught up when you closed and
reopened the tray. A/C and Defrost looked dead for the same reason. Each control was asking the car
what it was set to before deciding what to send, and the car answers a beat late — so several quick
presses all read the same old value. They now count from what was just sent.

**Choose your own tray buttons.**
The vehicle row in the quick tray was fixed at A/C, Defrost and Rear. Pick up to four from every
control the car has, **daytime lights** included — Settings › Quick buttons. Each one tells you
whether it can show its state, since some controls the car never reports back.

**Defrost F and Defrost R now say what they are:** Windscreen demist and Rear window heater.

**A background appears as soon as you choose it.**
It used to need a trip through a few other screens before it showed up.

**Split screen puts your apps back where they were.**
Coming back from the car's own settings left the panes empty even though the apps were still
running. They are now moved back into their panes with whatever they were doing intact — the video
still loaded, the route still set.

**And it asks before replacing them.** Opening a saved layout closes whatever is in the split; it now
warns and names what it is about to close.

---

## 1.98 — 15 August 2026

**You can see the update downloading.**
There is a progress bar with a percentage now. Before this the screen said "Downloading…" and then
nothing changed, so there was no way to tell a slow connection from a stuck one.

**"Later" means later, not never.**
If you dismiss an update it comes back the next day. Before, dismissing it once meant you were never
asked again and had to find it yourself in Settings. **Skip this version** still means never — that
is what it is for.

**The cabin fan goes all the way to 10.**
It stopped at 7, three steps short of what the car's own climate panel does, so the top of the fan
range could not be reached from the app at all.

---

## 1.97 — 14 August 2026

**Add and remove home tiles.**
Tap ✎ on the home screen, then **+** to add a widget, an app shortcut, Now playing, Cabin or
Navigation. Hold any tile to remove it. Until now you could move, resize and fill tiles but not
change which ones were there — the only way was to switch to a different layout. Removing a tile
closes the gap instead of leaving a hole, and Home setup can bring back anything you removed.

**Split screen keeps your apps running.**
Leaving the split for the car's own launcher and coming back used to restart everything. Maps and
YouTube now come back where you left them.

**The quick tray's climate buttons work.**
A/C, Defrost and Rear were sending the wrong thing to the car and had quietly done nothing for a
long time. They also light up now to match what the car is actually doing.

**Navigation HUD text no longer overlaps.**
On smaller placements the arrival time ran into everything beside it. The HUD now drops what does
not fit instead of shrinking it past the point of being readable.

**Menus open where you are looking.**
In All Apps, holding an app, opening a folder's menu, choosing another screen or picking a group all
used to appear in the middle of the display. They now drop down next to whatever you pressed.

**The split Layout button gets out of the way.**
It sat over the top of your apps permanently. It now fades to a small mark a few seconds after you
last used it, and still opens with one tap.

**Updates install while you are driving.**
They used to be refused until the car stopped. You are now told what will happen — the launcher
restarts, and the instrument cluster goes dark for a few seconds if you have it turned on — and you
decide. Nothing installs without you agreeing.

**New: an optional way to help.**
**Settings › Privacy** has a switch, off unless you turn it on, that sends counts once a day — how
often screens are opened, and which buttons the car did not respond to. That last one is the point:
the climate buttons above were broken for months because a button that silently does nothing looks
exactly like a button nobody pressed. Your location, routes, speed, media and installed apps are
never sent, and there is no third-party tracking in the app. The screen lists all of it.

---

## 1.92 — 11 August 2026

**It now appears in your app list.**
On some cars the icon was missing after installing, because the system hides apps that can act as a
home screen. There is a normal app icon now, so you can always open it.

**Drag to reorder.**
Quick-tray buttons are rearranged by dragging the ≡ grip instead of tapping arrows.

**Automatic updates.**
The app checks for new versions on its own and tells you when one is ready. It still only installs
when you agree, and never while the car is moving.

**A proper sign-in page**, and an account that backs up more.
Rail order, tray settings, split presets, app groups, saved zones, cluster setup and calibration are
all included now — several of them were quietly being left out.

**Simpler cluster layouts.**
Full, Free and Zones, and you can now save your own arrangement as a named preset instead of picking
from fixed ones you could not change.

**Fixed**
- The instrument strip faded between taps — the system was forcing our layer to 80% opacity.
- Maximising one app in split screen closed the others.
- An empty split pane showed black instead of your background, and could not be filled again.
- Recent apps show real thumbnails of each app, in a carousel.
- Menus no longer refuse to open while the car is moving. Vehicle controls still do.
- The tray could be missing after a first install.

---

## 1.84 — 10 August 2026 · first public release

**Your instrument cluster, your way.**
Replace the factory gauge with your own scene, palette and layout, or keep the factory one and add
widgets around it. Speed, gear, range, tyre pressures and navigation guidance come from the car
itself.

**A home screen you compose.**
Icons down one side and a centre you fill yourself. Tap **✎** in the corner and the layout becomes
editable in place: drag tiles to move them, drag a corner to resize, hold one to put an app in it or
pin it so nothing can push it out of the way.

**Every screen, used properly.**
Split the main screen between two or three apps at whatever sizes suit you, save those as presets,
and send any app to any screen from the app drawer.

**Now playing, properly.**
Real album art, a progress bar and working skip controls. Tapping it opens whichever app is actually
playing.

**Open apps with real thumbnails.**
Recents shows the actual screen of each running app, in a carousel you can flick through. Swipe a
card away to close it and give the memory back.

**The bits that were missing.**
A floating Back button — or an edge swipe — that works over any app. A quick tray on the screen edge
for instant access to apps and controls. An app drawer with folders, sorting and search.

**Vehicle controls and macros.**
Climate, windows, lights and mirrors from one panel, plus macros that chain several actions into one
press — like leaving the car running and locked while you step out.

**Make it yours.**
A background image with adjustable frost and darkness, glass tiles you can make as solid or as
see-through as you like, accent colours and interface scale.

**Automatic updates.**
The app tells you when a new version is out and can install it for you. It only ever installs with
your permission, and never while the car is moving.

**An optional account.**
Backs up your layouts, presets and macros so a reinstall — or a second car — comes back exactly as
you left it. Everything works without one, for as long as you like. Sign-in is a code by email;
there is no password to remember.

---

### Privacy

- **Vehicle data never leaves the car.** Speed, location, doors, tyres — all of it stays on the head
  unit.
- **The update check sends nothing about you or your car.** It reads a public list of releases.
- The optional account stores only your own settings. No telemetry, no advertising.
