# REAPER Script Cleanup Project

## Before You Begin
**Read these two files first:**
1. `/Users/jahammersmith/projects/my-lua-scripts/CLAUDE.md` - Lua scripting workflow and folder structure
2. `/Users/jahammersmith/projects/ipad-osc-surface/CLAUDE.md` - OSC surface project for iPad control

---

## Purpose
This project tracks the cleanup and organization of 288 Lua scripts currently in the Development folder. As scripts are tested and moved to permanent folders, they will be marked complete here.

## Workflow
1. **Test** - Run the script in REAPER to verify functionality
2. **Fix** - If broken, fix the script and re-test
3. **Sort** - Move working scripts to appropriate permanent folder with `ALDENHammersmith_` prefix
4. **Track** - Update spreadsheet and strike from this list

## Permanent Folder Categories
```
01. Automation Items    17. Meta                  33. Takes Properties
02. Autosampling        18. MIDI                  34. Templates
03. Batch Processing    19. MIDI Editor           35. Tempo and Time Signature
04. Color               20. MIDI Inline Editor    36. Time Selection
05. Composing           21. Mixing                37. Text Items and Item Notes
06. Cursor              22. Navigation            38. Theme
07. Development         23. Project               39. Tracks
08. Diagnostics & Debug 24. Razor Edit            40. Track Properties
09. Envelopes           25. Regions               41. Transport
10. Functions           26. Rendering             42. UI (RealmGui)
11. FX                  27. Routing               43. Various
12. FX Specific         28. Ruler                 44. Video
13. Items Editing       29. Sample Libraries      45. View
14. Items Properties    30. Spectral Edits        46. Web Interfaces
15. Markers             31. Stretch Markers       47. Workflows (Cross-cutting)
16. Media Explorer      32. Subprojects
```

---

## Script Inventory (288 total)

### Legend
- [ ] Not tested yet
- [x] ~~Script Name~~ - Moved to permanent folder
- [!] Broken - needs fix

---

### 01_MIDI Scripts (28 scripts)

#### Toggle Pencil and Lasso
- [ ] `Toggle Pencil and Lasso for Midi Editor_v001.lua`

#### Toggle Midi CC 011 Lane
- [x] ~~`Toggle Midi CC 011 Lane_v001.lua`~~ DELETED (older version, permanent exists in 19. MIDI Editor)
- [x] ~~`Toggle Midi CC 011 Lane_v002.lua`~~ DELETED (was CC1 toggle, already in 19. MIDI Editor as CC01)
- [x] ~~`Toggle Midi CC 011 Lane_v003.lua`~~ DELETED (duplicate of permanent)

#### Quantize Selected Midi Notes End to Forward Grid
- [ ] `Quantize Selected Midi Notes End to Forward Grid_v001.lua`

#### Quantize Midi Velocity Max
- [x] ~~`Quantize Selected Midi Note Max Velocity100_v001.lua`~~ → 18. MIDI
- [x] ~~`Quantize Selected Midi Note Max Velocity120_v001.lua`~~ → 18. MIDI
- [x] ~~`Quantize Selected Midi Note Max Velocity20_v001.lua`~~ → 18. MIDI
- [x] ~~`Quantize Selected Midi Note Max Velocity40_v001.lua`~~ → 18. MIDI
- [x] ~~`Quantize Selected Midi Note Max Velocity60_v001.lua`~~ → 18. MIDI
- [x] ~~`Quantize Selected Midi Note Max Velocity80_v001.lua`~~ → 18. MIDI

#### Midi Velocity Compressor
- [x] ~~`Midi Velocity Compressor 20%_v001.lua`~~ → 18. MIDI
- [x] ~~`Midi Velocity Compressor 30%_v001.lua`~~ → 18. MIDI
- [x] ~~`Midi Velocity Compressor 5%_v001.lua`~~ → 18. MIDI
- [x] ~~`Midi Velocity Compressor 50%_v001.lua`~~ → 18. MIDI
- [x] ~~`Midi Velocity Linear Compressor Slider_v001.lua`~~ → 18. MIDI

#### Reduce Midi Velocity by Percent
- [ ] `Reduce Midi Velocity by Percentage_v001.lua`

#### Midi cc64 Hold Pedal
- [ ] `Midi cc64 Hold Pedal_Pedal off 1 beat_v001.lua`
- [ ] `Midi cc64 Hold Pedal_Pedal off 1 beat_v002.lua`

#### Fill note ends to the start of next note
- [ ] `Fill note ends to the start of next note_001.lua`
- [ ] `Fill note ends to the start of next note_002.lua`

#### Make Monophonic Legato
- [ ] `Make Monophonic Legato_002.lua`

#### Shorten Midi Ends 25ms
- [ ] `Shorten Selected Midi Ends 25 ms_001.lua`

#### Nudge Selected Midi Notes Back 100 ms
- [ ] `Nudge Selected Midi Notes Back 100 ms_001.lua`

#### Convert Pedal to sustain midi notes
- [ ] `Convert Pedal to sustain midi notes_v001.lua`

#### Select all Midi Notes in Project
- [ ] `Select all Midi Notes in Prroject_v001.lua`

#### Transpose Project Midi
- [ ] `Transpose Project Midi +1 Semitone_v001.lua`
- [ ] `Transpose Project Midi -1 Semitone.lua`

---

### 03_Transport Scripts (5 scripts)

#### Transport Playhead 1 Measure
- [x] ~~`Transport Playhead 1 Measure_v001.lua`~~ DELETED (duplicate)
- [x] ~~`Transport Playhead Forward 1 Measure_v001.lua`~~ → 41. Transport
- [x] ~~`Transport Playhead Backward 1 Measure_v001.lua`~~ → 41. Transport

#### Toggle to Next Used Midi Track
- [ ] `Forward Toggle to Next  Used Midi Track_001.lua`
- [ ] `Backward Toggle to Next Used Midi Track_001.lua`

#### Advance/Regress 10 measures (root level)
- [ ] `Advance 10 measures.lua`
- [ ] `Advance playhead 10 measures.lua`
- [ ] `Regress playhead 10 measures.lua`

---

### 09_Tracks Scripts (12 scripts)

#### Toggle Hide/View All Unused Tracks
- [ ] `Expand all children tracks if children tracks are used small view.lua`
- [ ] `Expand all children tracks if children tracks are used small view_02.lua`
- [ ] `Expand all children tracks if children tracks are used.lua`
- [ ] `Uncollapse all folder stacks.lua`
- [x] ~~`001. Toggle Hide:View All Unused Tracks_001.lua`~~ DELETED (old version)
- [x] ~~`001. Toggle Hide:View All Unused Tracks_002.lua`~~ DELETED (old version)
- [x] ~~`001. Toggle Hide:View All Unused Tracks_003.lua`~~ DELETED (old version)
- [x] ~~`Toggle Hide:View All Unused Tracks_004.lua`~~ DELETED (old version)
- [x] ~~`Toggle Hide:View All Unused Tracks_005.lua`~~ DELETED (old version)
- [x] ~~`Toggle Hide:View All Unused Tracks_006.lua`~~ DELETED (old version)
- [x] ~~`Toggle Hide:View All Unused Tracks_007.lua`~~ → 39. Tracks

#### Search Track
- [ ] `Search Track.lua`

---

### 11_Render_Export Scripts (6 scripts)

#### Clear Regions from Render Matrix
- [ ] `Clear Selected Regions from Render Matrix_v001.lua`
- [ ] `Clear All Regions from Render Matrix_v002.lua`
- [ ] `Clear All Regions from Render Matrix_v003.lua`
- [ ] `Clear All Regions from Render Matrix_v004.lua`
- [ ] `Clear All Regions from Render Matrix_v005.lua`
- [ ] `-- Clear All Regions from Render Matrix_v006.lua`

---

### 16_Composing Scripts (72 scripts)

#### Select Voicing from Selected Notes
- [ ] `Select Voicing from Selected Notes_v001.lua`
- [ ] `Select Voicing from Selected Notes_v002.lua`

#### Build Midi into Seperate LUA Editor (v001-v038)
- [ ] `Build Midi into Seperate LUA Editor_v001.lua`
- [ ] `Build Midi into Seperate LUA Editor_v002.lua`
- [ ] `Build Midi into Seperate LUA Editor_v003.lua`
- [ ] `Build Midi into Seperate LUA Editor_v004.lua`
- [ ] `Build Midi into Seperate LUA Editor_v005.lua`
- [ ] `Build Midi into Seperate LUA Editor_v006.lua`
- [ ] `Build Midi into Seperate LUA Editor_v007.lua`
- [ ] `Build Midi into Seperate LUA Editor_v008.lua`
- [ ] `Build Midi into Seperate LUA Editor_v009.lua`
- [ ] `Build Midi into Seperate LUA Editor_v010.lua`
- [ ] `Build Midi into Seperate LUA Editor_v011.lua`
- [ ] `Build Midi into Seperate LUA Editor_v012.lua`
- [ ] `Build Midi into Seperate LUA Editor_v013.lua`
- [ ] `Build Midi into Seperate LUA Editor_v014.lua`
- [ ] `Build Midi into Seperate LUA Editor_v015.lua`
- [ ] `Build Midi into Seperate LUA Editor_v016.lua`
- [ ] `Build Midi into Seperate LUA Editor_v017.lua`
- [ ] `Build Midi into Seperate LUA Editor_v018.lua`
- [ ] `Build Midi into Seperate LUA Editor_v019.lua`
- [ ] `Build Midi into Seperate LUA Editor_v020.lua`
- [ ] `Build Midi into Seperate LUA Editor_v021.lua`
- [ ] `Build Midi into Seperate LUA Editor_v022.lua`
- [ ] `Build Midi into Seperate LUA Editor_v023.lua`
- [ ] `Build Midi into Seperate LUA Editor_v024.lua`
- [ ] `Build Midi into Seperate LUA Editor_v025.lua`
- [ ] `Build Midi into Seperate LUA Editor_v026.lua`
- [ ] `Build Midi into Seperate LUA Editor_v027.lua`
- [ ] `Build Midi into Seperate LUA Editor_v028.lua`
- [ ] `Build Midi into Seperate LUA Editor_v029.lua`
- [ ] `Build Midi into Seperate LUA Editor_v030.lua`
- [ ] `Build Midi into Seperate LUA Editor_v031.lua`
- [ ] `Build Midi into Seperate LUA Editor_v032.lua`
- [ ] `Build Midi into Seperate LUA Editor_v033.lua`
- [ ] `Build Midi into Seperate LUA Editor_v034.lua`
- [ ] `Build Midi into Seperate LUA Editor_v035.lua`
- [ ] `Build Midi into Seperate LUA Editor_v036.lua`
- [ ] `Build Midi into Seperate LUA Editor_v037.lua`
- [ ] `Build Midi into Seperate LUA Editor_v038.lua`
- [ ] `Untitled.lua`

#### Build Midi into Seperate LUA Editor (v1.028.xxx series)
- [ ] `Build Midi into Seperate LUA Editor_v1.028.001.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.002.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.003.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.004.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.005.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.006.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.007.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.008.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.009.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.010.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.011.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.012.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.013.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.014.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.015.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.016.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.017.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.018.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.019.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.020.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.021.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.022.lua`
- [ ] `Build Midi into Seperate LUA Editor_v1.028.023.lua`

#### Build Midi into Seperate LUA Editor V002 (v2.xxx series)
- [ ] `Build Midi into Seperate LUA Editor_v2.001.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.002.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.003.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.004.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.005.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.006.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.007.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.008.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.009.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.010.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.011.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.012.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.013.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.014.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.015.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.016.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.017.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.018.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.019.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.020.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.021.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.022.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.023.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.024.lua`
- [ ] `Build Midi into Seperate LUA Editor_v2.025.lua`

---

### 17_Timeline Scripts (5 scripts)

#### Time Signature
- [ ] `Insert 4:4 Time Signature at Playhead_v001.lua`
- [ ] `Insert 4:4 Time Signature at Playhead_v002.lua`
- [ ] `Insert 5:4 Time Signature at Playhead_v001.lua`
- [ ] `Insert 5:4 Time Signature at Playhead_v002.lua`

#### Tempo Mapping
- [ ] `Generate tempo and time signature on midi_v001.lua`

---

### AUTO SAMPLER SCRIPTS (62 scripts)

#### MIDI Sampler Full 88 Keys (main series v001-v025)
- [ ] `MIDI Sampler Full 88 Keys (Velocity Layers)_001.lua`
- [ ] `MIDI Sampler Full 88 Keys (Velocity Layers)v_002.lua`
- [ ] `MIDI Sampler Full 88 Keys (Velocity Layers)v_003.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range & Velocity Layers)v_004.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq)v_005.lua`
- [ ] `IDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq)v_006.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq)v_007.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type) v_008.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type)v_009.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type) v_010.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type)v_011.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type) v_012.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type, Pitch-Based Decay)v_013.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type, Round Robins)v_014.lua`
- [ ] `IDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type, Round Robins, Sudo-Logarithmic Decay) v_015.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type, Round Robins, Sudo-Logarithmic Decay Extreme)v_016.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type, Round Robins, Logarithmic Decay) v_017.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type, Round Robins, Aggressive Logarithmic Decay) v_018.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type, Round Robins, Balanced Decay) v_019.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type, Round Robins, Balanced Decay, Regions) v_020.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type, Round Robins, Regions w: Rest) v_021.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type, Round Robins, Regions, User Last Velocity) v_022.lua`
- [ ] `Name- MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type, Round Robins, Regions, User Last Velocity, Velocity Fix) v_023.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type, Round Robins, Regions, User Last Velocity, Velocity 127 Unique) v_024.lua`
- [ ] `MIDI Sampler Full 88 Keys (Prompted Range, Velocity, Sample Freq, Instrument Type, Round Robins, Regions, User Last Velocity, Velocity 127 Unique, Tight Length) v_025.lua`

#### Claude Version (v001-v029)
- [ ] `Midi Auto Sampler_v001.lua`
- [ ] `Midi Auto Sampler_v002.lua`
- [ ] `Midi Auto Sampler_v003.lua`
- [ ] `Midi Auto Sampler_v004.lua`
- [ ] `Midi Auto Sampler_v005.lua`
- [ ] `Midi Auto Sampler_v006.lua`
- [ ] `Midi Auto Sampler_v007.lua`
- [ ] `Midi Auto Sampler_v008.lua`
- [ ] `Midi Auto Sampler_v009.lua`
- [ ] `Midi Auto Sampler_v010.lua`
- [ ] `Midi Auto Sampler_v011.lua`
- [ ] `Midi Auto Sampler_v012.lua`
- [ ] `Midi Auto Sampler_v013.lua`
- [ ] `Midi Auto Sampler_v014.lua`
- [ ] `Midi Auto Sampler_v015.lua`
- [ ] `Midi Auto Sampler_v016.lua`
- [ ] `Midi Auto Sampler_v017.lua`
- [ ] `Midi Auto Sampler_v018.lua`
- [ ] `Midi Auto Sampler_v018a.lua`
- [ ] `Midi Auto Sampler_v019.lua`
- [ ] `Midi Auto Sampler_v020.lua`
- [ ] `Midi Auto Sampler_v021.lua`
- [ ] `Midi Auto Sampler_v022.lua`
- [ ] `Midi Auto Sampler_v023.lua`
- [ ] `Midi Auto Sampler_v028.lua`
- [ ] `Midi Auto Sampler_v028a.lua` (Gemini subfolder)
- [ ] `Midi Auto Sampler_v028b.lua`
- [ ] `Midi Auto Sampler_v028c.lua`
- [ ] `Midi Auto Sampler_v028d.lua`
- [ ] `Midi Auto Sampler_v028e.lua`
- [ ] `Midi Auto Sampler_v028f.lua`
- [ ] `Midi Auto Sampler_v029.lua`

#### Gemini Version
- [ ] `Midi Auto Sampler_v026.lua`
- [ ] `Midi Auto Sampler_v027.lua`

#### Cut Audio using Midi Note Start
- [ ] `Cut Audio using Midi Note Start_v001.lua`

---

### Midi Auto Sampling Scripts (17 scripts)

#### Cutting scripts
- [ ] `Glue and Cut Audio at MIDI Notes_v03.lua`
- [ ] `Cut Midi Samples_v04.lua`
- [ ] `Cut Midi Samples_v04_02.lua`

#### Trim silence scripts
- [ ] `Trim silence script_v01.lua`
- [ ] `Trim and move silence_v02.lua`
- [ ] `Trim and move silence_v03.lua`
- [ ] `Trim and move silence_v04.lua`
- [ ] `Trim and move silence_v05.lua`
- [ ] `Trim and move silence_v05_02.lua`
- [ ] `Trim and move silence from clip(for loop all clips)_v01.lua`
- [ ] `Trim and move silence starting from selected clip_06.lua`
- [ ] `Trim and move silence_v07.lua`
- [ ] `RMS calculate point for Trim and move silence_001.lua`
- [ ] `RMS calculate point for Trim and move silence_002.lua`

#### RMS detector
- [ ] `Measure RMS from playhead_v01.lua`
- [ ] `Measure RMS from Playhead_v02.lua`
- [ ] `Measure RMS from playhead_03.lua`

---

### Render Region Scripts (9 scripts)

#### Region Render Selector
- [ ] `001. Region Render Selector_v001.lua`
- [ ] `001. Region Render Selector_v002.lua`
- [ ] `001. Region Render Selector_v003.lua`

#### Select Render Regions in Track
- [ ] `001. Select Render Regions in Track_v001.lua`
- [ ] `001. Select Render Regions in Track_v002.lua`
- [ ] `001. Select Render Regions in Track_v003.lua`
- [ ] `001. Select Render Regions in Track_v004.lua`
- [ ] `001. Select Render Regions in Track_v005.lua`
- [ ] `001. Select Render Regions in Track_v006.lua`

---

### 1000_Alden's Custom Scripts (12 scripts)

#### Select All Regions from Determined Track
- [ ] `Select All Regions from Determined Track_v001.lua`

#### Auto Hide children tracks on folder collapse
- [ ] `Auto Folder MCP Hider_v002.lua`
- [ ] `Auto Hide children tracks on Folder Collapse_v001.lua`
- [ ] `Auto Hide children tracks on Folder Collapse_v003.lua`
- [ ] `Auto Hide children tracks on Folder Collapse_v004.lua`
- [ ] `Auto Hide children tracks on Folder Collapse_v005.lua`
- [ ] `Auto Hide children tracks on Folder Collapse_v006.lua`
- [ ] `Auto Hide children tracks on Folder Collapse_v007.lua`
- [ ] `Auto Hide children tracks on Folder Collapse_v008.lua`

#### Unique Scripts
- [ ] `Smart Propogate ReaControlMidi_v001.lua`
- [ ] `Smart Propogate ReaControlMidi_v002.lua`
- [ ] `Remove ReaControlMidi from All Tracks_v001.lua`
- [ ] `Copy ReaControlMidi to All Tracks_v001.lua`

---

### Fades Scripts (1 script)
- [ ] `Remove start fades on selected items_v01.lua`

---

### Root Level Scripts (15 scripts)
- [ ] `Sampler script gen1.lua`
- [ ] `PianoAutoSampler_Velocityfreq10s_3RoundRobins.lua`
- [ ] `AutoSampleEditor_v001.lua`
- [ ] `AutoSetup_Neve88M_AudioBox_MIDI.lua`
- [ ] `Cut Samples at MIDI Notes.lua`
- [ ] `Test ReaImGui.lua`
- [ ] `check presence for reaper.imgui.lua`
- [ ] `test is any extension here.lua`
- [ ] `test imgui issue.lua`
- [ ] `test please work verify imgui install.lua`
- [ ] `sandbox tester.lua`
- [ ] `workflow-test.lua`
- [ ] `workflow-test2.lua`
- [ ] `_add-to-action-list.lua` (HELPER - keep in Development)
- [ ] `register_script.lua` (HELPER - keep in Development)

---

### "These need sorted" Folder (24 scripts - DUPLICATES)
*These appear to be copies of scripts from 01_MIDI. Verify and delete duplicates.*

- [x] ~~`ALDENHammersmith_Toggle Midi Lane CC11.lua`~~ DELETED (duplicate of 19. MIDI Editor version)
- [ ] `Quantize Selected Midi Notes End to Forward Grid.lua`
- [x] ~~`Quantize Selected Midi Note Max Velocity100_v001.lua`~~ DELETED (duplicate)
- [x] ~~`Quantize Selected Midi Note Max Velocity120_v001.lua`~~ DELETED (duplicate)
- [x] ~~`Quantize Selected Midi Note Max Velocity20_v001.lua`~~ DELETED (duplicate)
- [x] ~~`Quantize Selected Midi Note Max Velocity40_v001.lua`~~ DELETED (duplicate)
- [x] ~~`Quantize Selected Midi Note Max Velocity60_v001.lua`~~ DELETED (duplicate)
- [x] ~~`Quantize Selected Midi Note Max Velocity80_v001.lua`~~ DELETED (duplicate)
- [x] ~~`Midi Velocity Compressor 20%_v001.lua`~~ DELETED (duplicate)
- [x] ~~`Midi Velocity Compressor 30%_v001.lua`~~ DELETED (duplicate)
- [x] ~~`Midi Velocity Compressor 5%_v001.lua`~~ DELETED (duplicate)
- [x] ~~`Midi Velocity Compressor 50%_v001.lua`~~ DELETED (duplicate)
- [x] ~~`Midi Velocity Linear Compressor Slider_v001.lua`~~ DELETED (duplicate)
- [ ] `Reduce Midi Velocity by Percentage_v001.lua`
- [ ] `Midi cc64 Hold Pedal_Pedal off 1 beat_v001.lua`
- [ ] `Midi cc64 Hold Pedal_Pedal off 1 beat_v002.lua`
- [ ] `Fill note ends to the start of next note_001.lua`
- [ ] `Fill note ends to the start of next note_002.lua`
- [ ] `Make Monophonic Legato_002.lua`
- [ ] `Shorten Selected Midi Ends 25 ms_001.lua`
- [ ] `Nudge Selected Midi Notes Back 100 ms_001.lua`
- [ ] `Convert Pedal to sustain midi notes_v001.lua`
- [ ] `Select all Midi Notes in Prroject_v001.lua`
- [ ] `Transpose Project Midi +1 Semitone_v001.lua`
- [ ] `Transpose Project Midi -1 Semitone.lua`

---

## Progress Summary
- **Total Scripts:** 288
- **Tested:** 21
- **Moved to Permanent:** 14
- **Deleted:** 22
- **Broken/Needs Fix:** 0
- **Remaining:** 252

---

## Session Log
*Record testing sessions here*

### 2026-01-15
- Created cleanup tracking project
- Inventoried all 288 scripts
- Tested and moved Transport Playhead Forward 1 Measure → 41. Transport
- Tested and moved Transport Playhead Backward 1 Measure → 41. Transport
- Deleted duplicate Transport Playhead 1 Measure_v001.lua
- Tested and moved Toggle Hide:View All Unused Tracks_007 → 39. Tracks
- Deleted 6 older versions of Toggle Hide/View script (001-006)
- Created OSC button "Show/Hide Unused Tracks" (p1_view_unusedtracks)
- Updated all spreadsheets and OSC bindings
- Moved 5 Midi Velocity Compressor scripts → 18. MIDI
- Created 5 OSC buttons on Page 2 for velocity compressors
- Deleted 5 duplicate velocity compressor scripts from "These need sorted"
- Moved 6 Quantize Midi Velocity Max scripts → 18. MIDI
- Created 6 OSC buttons on Page 2 for velocity max (row 2)
- Deleted 6 duplicate velocity max scripts from "These need sorted"
- Deleted Toggle Midi CC 011 Lane_v001.lua (older version)
- Deleted Toggle Midi CC 011 Lane_v003.lua (duplicate of permanent)
- Deleted ALDENHammersmith_Toggle Midi Lane CC11.lua from "These need sorted" (duplicate)
- Note: v002 is mislabeled - actually CC1 (Mod Wheel) toggle, not CC11
- Deleted v002 (CC01 already finalized in 19. MIDI Editor)
- Added Toggle CC11 and Toggle CC01 buttons to Page 2 of OSC layout
- Added ALDENHammersmith_Toggle Midi Lane CC01.lua to GitHub
- Added ALDENHammersmith_Toggle Midi Lane CC11.lua to GitHub

