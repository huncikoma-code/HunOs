[README.md](https://github.com/user-attachments/files/32142044/README.md)
# HUN OS 1.0

A very small web desktop with a 1996 face. No build step, no dependencies,
no framework — a single HTML file holding the markup, the styles and the
script together.

## Running it

Double-click `index.html`. Nothing else is needed

## Starting up

The first screen is an Obi-Wan Kenobi "Hello there." picture with **Welcome**
underneath. Click anywhere, or press any key, and you are on the desktop.
There is no boot animation and no password prompt.

### The picture

The start screen loads the still from a remote address, set on the `<img>`
tag near the top of `index.html`. Change that `src` to swap the picture —
a URL or a local file name both work.

## The desktop

- **Icons can be dragged** anywhere on the desktop. Where you drop them is
  remembered, so the layout survives a reload.
- Double-click an icon to start the program; a single click just selects it.
- **Right-click empty desktop** opens Display Properties.

## Programs

| Program | What it does |
|---|---|
| **Calculator** | Four operations, C / CE / backspace, keyboard input as well |
| **HunNet Navigator** | Internal `hun://` pages (home, catalog, Jedi Archive, guestbook, help), history, and real web addresses too |
| **Notepad** | Editing, save/open through browser storage, time/date insert, word wrap toggle |
| **MS-HUN Command Prompt** | `HELP`, `DIR`, `TYPE`, `MATH`, `ECHO`, `DATE`, `TIME`, `VER`, `WHOAMI`, `FORCE`, `HELLO`, `NEOFETCH`, `CLS`, `CALC`, `NOTEPAD`, `NET`, `DISPLAY`, `EXIT` — arrow keys walk the history |
| **Display Properties** | Pick your own wallpaper from a file, choose Stretch / Center / Tile, or remove it |

Windows drag by their title bar, minimize, maximize (double-click the title
bar) and close. Every running program appears on the taskbar, and everything
can be started from the Start menu.

## Files

- `index.html` — everything: the screens, the 90s stylesheet and the script

## Worth knowing

- Notes, guestbook entries, icon positions and the wallpaper live in the
  browser `localStorage`, so they are per-browser and per-machine.
- A chosen wallpaper is scaled down to at most 1600 px and stored as JPEG so
  it fits in that storage. Very large pictures still apply, but may be too big
  to remember after a reload — the window says so when that happens.
