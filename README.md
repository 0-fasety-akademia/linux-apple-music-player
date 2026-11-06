# Linux Apple Music Player

**Version 0.2.4 — 2026-11-06**

A fast, lightweight Apple Music player for Ubuntu. It has its own interface built directly on the Apple Music API; Apple's heavy web player is not loaded. Audio plays through Apple's MusicKit with Widevine, so full-length songs work with your subscription.

## Features

- Own lightweight UI, styled like Apple Music for Windows: sidebar, content area and player bar
- Sign in with your Apple ID (Apple Music subscription required)
- Home: recently played, heavy rotation and recommendations
- Radio: your personal station and Apple Music live radio
- Library: recently added, artists, albums, songs (infinite scroll) and your playlists in the sidebar
- Album, playlist and artist pages (top songs, albums, singles)
- Search in Apple Music or in your library (Ctrl+F)
- Right-click menu: play next, play later, add to library, add to playlist, go to album, copy link
- Queue panel with history; click a song to jump to it
- Cover view: large artwork, blurred background, all controls (Ctrl+Shift+L or click the song in the player bar)
- Synced lyrics in the cover view; click a line to jump to it
- Keyboard: Space play/pause, Ctrl+←/→ previous/next, Alt+← back, Esc closes panels
- Tray icon in the app's own style, light or dark following the system theme
- Tray menu with the current song and a small album cover, play/pause, next, previous
- Mouse wheel over the tray icon changes the volume
- Closing the window hides it to the tray; quit from the tray menu
- Ubuntu media controls (MPRIS): song, cover and controls in the top-bar menu and lock screen
- Media keys and `playerctl` work
- Optional notification for every new song, with cover (toggle in the tray menu)
- Light/dark theme follows the system; app and tray icons switch with it
- Dock right-click actions: Play/Pause, Next, Previous
- Polish UI when the system language is Polish, English otherwise
- Volume, window size and position are remembered; single instance
- Launching from a terminal detaches, so closing the terminal does not close the player

## Install

```bash
cd ~/Downloads
sudo apt install ./linux-apple-music-player_0.2.4_amd64.deb
```

Start **Linux Apple Music Player** from the app grid and sign in with your Apple ID.
The first launch downloads the Widevine DRM module from Google (a few seconds).

## Uninstall

```bash
sudo apt remove linux-apple-music-player
rm -rf ~/.config/linux-apple-music-player ~/.cache/linux-apple-music-player
rm -f ~/.local/share/icons/hicolor/*/apps/linux-apple-music-player.png
```

## Note

The app uses the public access key of Apple's own web player, as other third-party Apple Music clients do. This is not an official Apple API key; if Apple changes it, the app fetches the new one automatically, but Apple could block such use at any time.

## License

Free of charge to use and redistribute unmodified; modification is not permitted. See `LICENSE`.
Not affiliated with Apple Inc.

Created by: JGu  
Supported by Claude
