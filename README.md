# Hiraya Companion

The Gateway map for **Hiraya — The Lost Isle**, live on your second screen while you play The Isle: Evrima.

- Full Gateway map: water, food, AI, salt licks, gastroliths, migration and patrol zones, named locations
- A circular Mini Map that stays on top of the game (**Alt+M** to show or hide)
- Your position tracked automatically, read off your own screen — no alt-tabbing
- Pick the dinosaur you're playing and the map shows what it eats
- Waypoints, a breadcrumb trail, a nearest-location readout
- **Packs:** share your position with your packmates and see theirs, by invite code
- Marker packs: export your saved spots to a file and share them, import other people's

Server: <https://hirayeah.online/>

---

## Download

**[Latest release →](https://github.com/cyryljohn/hiraya-companion-public/releases/latest)**

Download `HirayaCompanion-Setup-<version>.exe` from the newest release and run it.

## Installing

1. Run the setup file. **No admin password is needed** — it installs just for your Windows account.
2. Windows may show a blue **"Windows protected your PC"** box. Click **More info → Run anyway**. That appears because the app isn't code-signed yet, not because anything is wrong with it. The SHA-256 of every installer is listed on its release page if you want to check the file.
3. Open **Hiraya Companion** from your desktop or Start menu. A short tour shows you around the first time.

Updating is the same: run the newer setup file over the old one. Your settings and saved markers are kept. The app tells you when a newer version is out.

## Getting your position on the map

**Copy your location** (works straight away): copy your location in game and your marker moves.

**OCR Tracking** (automatic): press **Tab** in game so your coordinates show, then in Hiraya click the arrow on **追跡 OCR TRACKING → Set up capture area** and drag a box around just the coordinate numbers. There's a picture in that window showing exactly what to select. From then on, keep the Tab menu open for about **3 seconds** and your marker updates; it reads the numbers off your screen about once a second and needs two matching reads before it moves you.

## Packs

In the sidebar under **群 PACK**, one player picks **Create a pack** and gets an 8-character code. Everyone else picks **Join with code**. Switch on **Share my position** and your packmates appear on both maps as named coloured dots; how long ago each was seen is written next to their name in the list.

- **Pack waypoint:** the leader places a waypoint, then **WAYPOINT ▸ Set as pack waypoint**. Everyone sees it as a gold diamond, and while **Follow pack waypoint** is on (it is when you join) it's your active waypoint — your distance and heading point at it, and it moves when the leader moves it.
- **Names and opacity:** hide packmates' names with the **Show names** switch or **Ctrl+Shift+N**; set how strong the pack layer is drawn in Settings › Map & Tracking › Pack.
- Share the code in **DMs, not a public channel** — anyone holding it can see the pack until the leader rotates it (**⋯ → Rotate code**).
- You only see your packmates **while you are sharing**, and sharing is off every time you start the app. Nobody can watch a pack silently.
- Positions are what each player's own app read from their screen — never from the game server.

## Is it safe? Will it get me banned?

**No.** Hiraya never reads or touches The Isle. It doesn't read game memory, doesn't modify game files, doesn't inject anything, doesn't hook the renderer, doesn't look at game traffic, and never sends input to the game. It only sees your clipboard and the pixels already on your screen — the same as taking a screenshot. The Mini Map is an ordinary window that happens to stay on top.

## What leaves your PC

- **Nothing**, by default.
- Once per launch, one small version file is fetched from this page's releases so the app can tell you a newer build exists. Nothing about you is sent. You can switch it off in Settings › Advanced.
- If you use **Packs**: your display name when you create or join, and your position **only while Share my position is on**, both only to the Hiraya server owner's pack service. There is no history — your latest position is overwritten, and deleted when you leave, are kicked, or stop sharing.

No account, no sign-in, no telemetry.

## Requirements

- Windows 10 or 11, 64-bit
- For OCR Tracking: a Windows OCR language pack (English is normally already installed)

## Troubleshooting

- **"Windows protected your PC"** — More info → Run anyway (see Installing).
- **Smart App Control refuses to run it at all** — some Windows 11 PCs have Smart App Control on, which blocks every unsigned program. Until the app is signed there's no way around that setting on that PC.
- **Two Hiraya windows / a Mini Map that won't close** — only one copy runs at a time; a second one just brings the first forward. Use the tray icon → **Exit** to close it fully.
- **OCR says it can't read** — make the capture box tight around the numbers only, and keep the Tab menu open a little longer.
- **No Windows OCR language** — Settings › Time & Language › Language › add English, or the language your game runs in, with the OCR feature.

Questions and bug reports: the Hiraya Discord.

---

This repository holds the downloads and this page only. The app's source is not published here.
