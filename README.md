# VST3
This is where i'm storing all of my VST3 addons for testing. they're all free, enjoy.

##INSTALLATION:

- Step 1: download the zip file.
- Step 2: open the zip file
- Step 3: open VST3-main
- Step 4: right click on Liberty Limiter 2.vst3 and copy the file. 
- Step 5: find your local VST3 file folder (you can open this in Ableton under Options, Settings, and clicking the "plugins" tab.) 
click browse paste the file in the folder and click "rescan" 

- To verify the VST is working click on the "liberty music ray" logo in the bottom and add some of my music to your playlists. 
why? because you love me and you want to support me and all of my bad habits!


# Liberty Limiter 2 - Quick User Guide

**Simple, honest guide to what's actually working right now.**

This plugin is still in development. The core limiting, visualizer, and most controls are usable. Some features are still under construction.

---

## Current Status

**Working:**
- Main audio limiting engine
- All the knobs listed below
- Visualizer (waveform + gain reduction history + exact limiting spots)
- Metering (GR, True Peak, LUFS M/S/I, LRA)
- Lookahead and oversampling
- A/B buttons
- Reset to Pass-Through button
- Basic MIDI Learn
- Power switch and most advanced toggles

**Still under construction:**
- Presets (save/load/delete system is not reliable yet)
- Full style differentiation (the 9 styles exist and sound different, but the deep per-style behaviors are still being refined)

---

## How to Use It

1. Load a **brand new instance** on a track (old instances can carry stale settings or latency).
2. On first load the plugin is designed to be completely transparent (pass-through). Nothing should happen to your audio.
3. Play audio. The big visualizer area will show the waveform.
4. To start limiting, lower the **THRESH** knob from 0 dB.
5. Use the big **Reset to Pass-Through** button (bottom strip) anytime you want to start fresh.

The plugin is intentionally transparent at default settings.

---

## Current Layout & Working Controls

### Top Row (Main Processing)
- **GAIN** (-24 dB to +14 dB)  
  Input gain before limiting. Negative = pull back, positive = drive harder.

- **THRESH** (-60 dB to 0 dB)  
  Main threshold. This is the primary control for how much limiting happens.

- **CEILING** (-20 dB to 0 dB)  
  Output brickwall level. The limiter works hard not to let peaks go above this.

- **MAKEUP** (0 dB to 20 dB)  
  Manual gain applied after limiting.

- **KNEE** (0 dB to 30 dB)  
  Soft knee width. 0 = hard brickwall. Higher values = smoother, more gradual limiting (similar to Ableton's knee behavior).

### Second Row (directly under the top row)
- **WIDTH** (0% to 500%)  
  Stereo width (mid/side).  
  0% = mono, 100% = normal stereo, higher = increasingly wide.  
  Placed directly under GAIN.

- **ATTACK** (0 ms to 30 ms)  
  How fast the limiter reacts to new peaks.

- **RELEASE** (10 ms to 2000 ms)  
  Base release time. Actual behavior is also influenced by the chosen style.

- **TRANSIENT** (0% to 100%)  
  Transient preservation. Higher values protect sharp attacks (drums, plucks, etc.) so they don't get squashed as hard.  
  This is **not** stereo width — it's about keeping punch and attack.

### Visualizer & Metering (the big area)
- Scrolling waveform + gain reduction curve.
- Orange/red vertical lines show the **exact spots** where limiting is occurring.
- Right-side bars for GR and True Peak with peak hold.
- Bottom text line shows live GR + True Peak + LUFS (Momentary / Short / Integrated) + LRA.

The visualizer is one of the more finished and useful parts of the plugin right now.

### Bottom Strip (Advanced Controls)
- **STYLE** selector (9 options currently)
- **OS** (Oversampling 1x–32x)
- **LOOK** (Lookahead 0–10 ms)
- Link Mode, Dither Type, Phase Mode (Min/Lin)
- Toggles: Auto Gain, Unity Gain, Audition GR, DC Filter, Dither
- **Reset to Pass-Through** button
- Basic preset navigation controls (still limited)

### Other Working Controls
- Large Power switch (top right)
- A/B comparison buttons
- MIDI Learn button (basic functionality)

---

## Quick Tips

- Start with everything at default, then lower **THRESH** until you see a few dB of gain reduction on peaks.
- Use **Lookahead** at 2–5 ms for most material.
- Use **TRANSIENT** if your drums or attacks are getting flattened.
- Use **WIDTH** if you want the sound to feel bigger spatially.
- Watch the red/orange lines in the visualizer — they show you exactly where the limiter is working.
- Hit **Reset to Pass-Through** often to compare before/after.

---

For now, treat this as a capable prototype. The limiting, visual feedback, and main controls are the strongest parts. Presets and deeper style work are the main things still being finished.
