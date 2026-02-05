# Kitty Keybindings Cheat Sheet

How to read sequences:
- `ctrl+a>k` means press `ctrl+a`, release, then press `k`.
- Same for `ctrl+shift+p>c` (press the prefix, then the next key).

Leader keys:
- `ctrl+a>` is the main tmux-like prefix.
- `kitty_mod` is `ctrl+shift` (used for some window navigation).

If you feel "stuck" in a vim-like layout:
- `alt+enter` toggles the stack layout (single-window focus vs splits).
- `ctrl+a>z` toggles zoom on the current pane.

## Windows / Panes (Splits)
- `ctrl+a>x` close current window (pane).
- `alt+w` close current window (pane).
- `alt+\` split vertically (vsplit, reuse cwd).
- `alt+ctrl+\` split horizontally (hsplit, reuse cwd).
- `ctrl+a>-` split horizontally (hsplit, reuse cwd).
- `ctrl+a>shift+-` split horizontally (hsplit, no cwd reuse).
- `ctrl+a>\` split vertically (vsplit, reuse cwd).
- `ctrl+a>shift+\` split vertically (vsplit, no cwd reuse).
- `f4` split automatically based on window shape.
- `alt+n` new OS window.
- `ctrl+q` close OS window.

## Window / Pane Navigation
- `ctrl+a>]` next window.
- `ctrl+a>[` previous window.
- `ctrl+a>h` focus left.
- `ctrl+a>j` focus down.
- `ctrl+a>k` focus up.
- `ctrl+a>l` focus right.
- `alt+ctrl+h` focus left.
- `alt+ctrl+j` focus down.
- `alt+ctrl+k` focus up.
- `alt+ctrl+l` focus right.
- `kitty_mod+left` focus left.
- `kitty_mod+right` focus right.
- `kitty_mod+up` focus up.
- `kitty_mod+down` focus down.
- `ctrl+a>q` focus by visible window label.

## Window / Pane Layout
- `alt+enter` toggle layout stack (single-window focus).
- `ctrl+a>z` zoom toggle for current pane.
- `f7` rotate split orientation.
- `ctrl+a>period` move window forward.
- `ctrl+a>comma` move window backward.
- `shift+up` move window up.
- `shift+down` move window down.
- `shift+left` move window left.
- `shift+right` move window right.
- `alt+ctrl+p` swap with another window.

## Resize Panes
- `alt+minus` resize shorter.
- `alt+equal` resize taller.
- `ctrl+home` reset pane sizes to defaults.

## Tabs
- `alt+t` new tab.
- `ctrl+a>c` new tab (reuse cwd).
- `alt+ctrl+w` close tab.
- `alt+[` previous tab.
- `alt+]` next tab.
- `alt+ctrl+[` move tab backward.
- `alt+ctrl+]` move tab forward.
- `ctrl+a>1`..`ctrl+a>9` go to tab 1..9.
- `ctrl+a>0` go to tab 10.
- `ctrl+a>,` set tab title.
- `alt+0` set tab title.
- `alt+9` toggle tab bar.

## Scrollback / Search / Hints
- `f1` show scrollback.
- `ctrl+a>space` hints (custom alphabet).
- `f3` hints for all programs.
- `alt+f` search scrollback with fzf overlay.
- `alt+ctrl+u` open URL with hints.

## Clipboard / Input Helpers
- `ctrl+shift+c` copy to clipboard.
- `ctrl+shift+v` paste from clipboard.
- `shift+enter` send literal newline.
- `ctrl+a>ctrl+a` send `ctrl+a` literal.

## Fonts / View
- `ctrl+minus` decrease font size.
- `ctrl+equal` increase font size.
- `ctrl+0` reset font size.
- `ctrl+shift+0` reset font size.
- `f11` toggle fullscreen.

## Config / Tools
- `ctrl+a>e` disabled (no-op).
- `ctrl+a>shift+e` open kitty.conf in nvim.
- `ctrl+a>shift+r` reload kitty.conf (overlay confirmation).
- `ctrl+a>shift+d` debug config (also `f12`).
- `f2` open kitty @ help overlay.
- `ctrl+a>s` save session (overlay confirmation).
- `ctrl+a>t` open theme switcher.
- `ctrl+shift+p>c` choose file.
- `ctrl+shift+p>d` choose directory.

Notes:
- `splits.conf` only applies cleanly when the layout is `splits`.
- Some bindings appear twice; the last definition in `kitty.conf` wins.
