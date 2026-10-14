# LaraMonster downloads

LaraMonster is a local PHP & Laravel development environment for **Linux, macOS and Windows**: every project on its own local address, every PHP version, HTTPS, MySQL / PostgreSQL / Redis / Mailpit / Meilisearch, a mail inbox and a new-project wizard. It's free.

**LaraMonster Pro** adds the Event Tracker and Jobs & Queues → [monstersgate.com/laramonster](https://monstersgate.com/laramonster)

This repository only holds the downloads.

## Install

Download the file for your computer from the [releases page](https://github.com/MahmoudAdelMansour/laramonster-releases/releases), or from [monstersgate.com/laramonster](https://monstersgate.com/laramonster).

LaraMonster isn't signed by Apple yet, and Windows doesn't know the plain `.exe` yet, so both warn you the first time you open it. That warning appears once; after that LaraMonster opens normally and updates itself without asking again.

### macOS (11 or newer, Apple Silicon and Intel)

1. Download **`LaraMonster-macos-universal.zip`** and double-click it to unzip.
2. Drag **LaraMonster** into your **Applications** folder. Open it from there; it can only update itself from Applications.
3. Double-click LaraMonster. macOS says *“Apple could not verify ‘LaraMonster’ is free of malware…”*. Click **Done** (not *Move to Trash*).
4. Open **System Settings → Privacy & Security** and scroll down to **Security**. Next to *“LaraMonster was blocked to protect your Mac”*, click **Open Anyway**.
5. Click **Open Anyway** once more and enter your Mac password. LaraMonster opens.

The **Open Anyway** button only shows for about an hour after step 3; if you don't see it, open LaraMonster again first. Right-click → Open no longer works for this on macOS 15 and newer.

Comfortable with the Terminal? This does steps 3–5 in one go:

```sh
xattr -dr com.apple.quarantine /Applications/LaraMonster.app
```

### Windows 10 and 11

**Microsoft Store (recommended):** [get LaraMonster from the Microsoft Store](https://apps.microsoft.com/detail/9NRLB8PVVP9X). No warnings, and the Store keeps it updated.

**Or the `.exe`:**

1. Download **`LaraMonster-windows-amd64.exe`**. If your browser says the file *isn't commonly downloaded*, choose **Keep**.
2. Move it to a folder of its own, for example `Documents\LaraMonster`, so it can update itself.
3. Double-click it. If Windows shows *“Windows protected your PC”*, click **More info**, then **Run anyway**.

### Linux (x86-64)

```sh
tar xzf LaraMonster-linux-amd64.tar.gz
./LaraMonster/install.sh
```

LaraMonster is then in your app menu, and `laramonster` works in new terminals. Nothing needs `sudo`: it installs into `~/.local/bin`.

### Updates

When you open LaraMonster it checks for a new version, then downloads and installs it by itself and asks you to **Restart** when it's ready (your sites pause for a few seconds). Prefer to decide yourself? Turn off **Settings → About → Update automatically**: LaraMonster then only tells you a new version is out, with an **Update now** button. Microsoft Store copies are updated by the Store.
