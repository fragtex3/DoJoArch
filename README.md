# 🥋 DOJO - Custom Arch Linux Hacking Distribution

```
╔═══════════════════════════════════════════════════════════════════════════╗
║                                                                           ║
║           🥋 CUSTOM ARCH LINUX - DOJO EDITION 🥋                        ║
║                                                                           ║
║  Professional Hacking Operating System with Custom Toolkit & Design      ║
║  Built for Security Professionals | Maintained as a Living Project      ║
║                                                                           ║
║  Status: ✅ READY FOR DEPLOYMENT                                        ║
║  Version: 1.0 Master Edition                                            ║
║  Last Updated: 2026-01-02                                               ║
║                                                                           ║
╚═══════════════════════════════════════════════════════════════════════════╝
```

---

## 📋 Was ist DOJO?

**DOJO** ist dein persönliches Hacking-Trainings-System – eine eigenständige Linux-Distribution basierend auf **Arch Linux**, mit:

- ✅ **Custom i3 Window Manager** mit deinem Branding
- ✅ **Automatisierter Installer** (alles in 30 Minuten)
- ✅ **Eigenes Panel-System** (Polybar-Ersatz)
- ✅ **Integriertes Security-Toolkit** (erweiterbar)
- ✅ **Professional Design** (Dunkelblau Theme + Cyan Accents)
- ✅ **Keyboard-optimiert** für Hacker & Professionals

**Ziel**: Ein Linux-System, das:
1. Genau so aussieht wie die BlackArch im Screenshot
2. Nur DEINE Tools und Scripts lädt
3. Vollständig scriptbar und deploybar ist
4. Als Trainingsbasis für dein Hacking-Abenteuer dient

---

## 🚀 Quick Start (5 Minuten)

### Option 1: Fresh Installation (Empfohlen)

```bash
# 1. Arch Linux installieren (https://archlinux.org/download/)
#    - USB-Stick mit ISO erstellen
#    - Von USB booten und standardmäßig installieren

# 2. Nach Reboot als normaler User:
git clone https://github.com/dein-username/dojo.git ~/dojo
cd ~/dojo
sudo ./install.sh

# 3. Neustarten und i3 beim Login wählen
reboot
```

**Dauer**: ~20-30 Minuten (inkl. 100+ Packages)

### Option 2: Zu bestehender Arch-Installation

```bash
# Wenn du schon Arch hast:
git clone https://github.com/dein-username/dojo.git ~/dojo
cd ~/dojo
sudo bash install.sh --components-only

# Instaliert nur i3, Panel, Configs (ohne base packages)
# Dauer: ~5 Minuten
```

---

## 📁 Projekt-Struktur

```
dojo/
├── README.md                    # Diese Datei
├── SETUP_GUIDE.md              # Detaillierte Anleitung (Phase 1-6)
├── SHORTCUTS.md                # Keyboard Shortcuts Referenz
├── INSTALL_SCRIPT.md           # Installation Details
│
├── install.sh                  # 🚀 HAUPTINSTALLER (ausführen!)
│
├── configs/
│   ├── i3/
│   │   └── config              # i3 Window Manager Config
│   ├── kitty/
│   │   └── kitty.conf          # Terminal Emulator Config
│   ├── rofi/
│   │   └── dojo-dark.rasi      # Application Launcher Theme
│   ├── picom/
│   │   └── picom.conf          # Compositor Config
│   ├── dunst/
│   │   └── dunstrc             # Notification Daemon Config
│   └── dojo/
│       ├── panel.py            # 🎨 CUSTOM PANEL SYSTEM
│       ├── startup.sh          # Startup Scripts
│       ├── aliases.sh          # Custom Aliases
│       └── colors.sh           # Color Definitions
│
├── scripts/
│   ├── setup-rust.sh           # Rust Environment Setup
│   ├── setup-shell.sh          # Zsh & Tmux Setup
│   └── update-system.sh        # System Update Script
│
├── templates/
│   ├── bash-tool-template.sh   # Template für Bash-Tools
│   ├── python-tool-template.py # Template für Python-Tools
│   └── rust-tool-template.rs   # Template für Rust-Tools
│
└── tools/
    └── (hier werden deine Custom Tools hinzugefügt)
```

---

## ⚙️ Installation Breakdown

Der `install.sh` macht folgendes:

### Phase 1: System Check (2 Sek)
- Verifiziert Arch Linux
- Prüft Root-Zugriff
- Kontrolliert Internet-Verbindung

### Phase 2: Package Installation (15 Min)
```
Core WM & Display:      i3-wm, rofi, feh, picom, xorg
Terminal & Shells:      kitty, zsh, tmux, bash-completion
Development:            git, rustup, python, nodejs, code
Utilities:              dunst, pavucontrol, pulseaudio, light
Security Tools:         nmap, netcat, tcpdump, wireshark, metasploit
Monitoring:             htop, nethogs, glances, lsof
Fonts:                  ttf-jetbrains-mono, ttf-hack, noto-fonts
```

### Phase 3: Configuration Setup (2 Min)
- Erstellt alle Config-Directories
- Kopiert i3, Rofi, Kitty Configs
- Generiert Systemd Services

### Phase 4: Shell Environment (3 Min)
- Installiert Zsh + Oh-my-zsh
- Konfiguriert Zsh Plugins
- Setzt ZSH als Default Shell

### Phase 5: Rust Toolchain (5 Min)
- Installiert Rust (für Custom Tools)
- Rrust Analyzer für Entwicklung

### Phase 6: Startup Scripts (1 Min)
- Erstellt Custom Startup-Scripts
- Generiert Aliases
- Initialisiert Git Repository

### Phase 7: Finalization (1 Min)
- Setzt Permissions
- Erstellt Desktop Entries
- Zusammenfassung anzeigen

---

## 🎨 Das Design

### Color Palette (DOJO Theme)

```css
/* Dark Base */
--bg-dark:        #0a0e27    (sehr dunkelblau)
--bg-lighter:     #1a1f3a    (dunkelblau mit glow)
--bg-accent:      #2a2f4a    (dunkler accent)

/* Text */
--fg-main:        #e0e6ff    (helles blau-weiß)
--fg-secondary:   #a0aacf    (mittleres blau)

/* Accents */
--accent-cyan:    #00d9ff    (neon cyan) ⭐ PRIMARY
--accent-blue:    #1e90ff    (royal blue)
--accent-red:     #ff4444    (warning rot)
--accent-green:   #00ff88    (success grün)
```

**Warum diese Farben?**
- ✅ Extreme Lesbarkeit (4.5:1+ Contrast Ratio)
- ✅ Hacker-Ästhetik (Matrix-vibes ohne Kitsch)
- ✅ Konsistent über alle Apps
- ✅ Accessibility-freundlich
- ✅ Terminal + IDE + Browser harmoniert

### Icons & Emojis

Workspaces verwenden Emojis:
```
1  ⌨️  Terminal         (Tippen & Hacking)
2  🔍 Reconnaissance   (Scanning & Enumeration)
3  🛠️  Tools           (Exploitation Framework)
4  📊 Monitoring       (Network Monitoring)
5  🔐 Exploitation     (Payloads & Exploitation)
6  📝 Notes            (Documentation)
7  🌐 Web              (Browser)
8  📁 Files            (File Manager)
9  ⚙️  System           (System Tools)
10 🎮 Other            (Sonstiges)
```

---

## 🎮 Keyboard Shortcuts

**Alle Shortcuts in `SHORTCUTS.md` dokumentiert**

### Essenzielle Shortcuts

```bash
# Launcher & Terminal
Mod+d               # Application Launcher (Rofi)
Mod+Return          # New Terminal (Kitty)
Mod+Ctrl+t          # Terminal + Tmux

# Workspace
Mod+1-9             # Goto Workspace 1-9
Mod+Shift+1-9       # Move Window to Workspace

# Window Management
Mod+h/v             # Split horizontal/vertical
Mod+f               # Fullscreen
Mod+j/k/l/;         # Focus Navigation (Vim-style)

# System
Mod+Shift+c         # Reload Config
Mod+Shift+r         # Restart i3
Mod+Shift+e         # Exit Session
```

Komplette Liste → siehe `SHORTCUTS.md`

---

## 🛠️ Custom Tools Integration

DOJO ist deine **Playground** für dein eigenes Toolkit!

### Tools hinzufügen

**Struktur:**
```
~/.local/share/dojo/tools/
├── nmap-quick          # Dein Script
├── port-scanner        # Dein Rust Binary
├── web-recon          # Dein Python Script
└── ...
```

**Beispiel: Bash-Tool erstellen**

```bash
mkdir -p ~/.local/share/dojo/tools
cat > ~/.local/share/dojo/tools/quick-scan << 'EOF'
#!/bin/bash
# Quick Nmap Scanner für DOJO
target=$1
echo "[+] Scanning $target..."
nmap -sV -sC -A -T4 $target
EOF

chmod +x ~/.local/share/dojo/tools/quick-scan
```

**Benutzen:**
```bash
Mod+d → quick-scan
# Oder direkt:
quick-scan target.com
```

### Beispiel Tools (zum selbst bauen)

1. **Port Scanner** (Python)
   - Multi-threaded Port Scanner
   - Service Detection
   - Report Generation

2. **Web Reconnaissance** (Rust)
   - Fast Subdomain Enumeration
   - Screenshot Generator
   - Archive.org Integration

3. **Payload Manager** (Python)
   - Exploit Database Manager
   - Custom Payload Generator
   - Version Control Integration

4. **Network Monitor** (Python)
   - Live Network Traffic Analysis
   - Protocol Detection
   - Alert System

---

## 📊 Custom Panel System

Das **panel.py** ist dein System-Monitor & Statusbar in einem:

```
[WS-1 | Workspace] ←--------────────────→ [CPU 45% | RAM 3.2/16GB | Temp 62°C | Vol 75% | 14:32:15]
```

### Panel Features

✅ **CPU-Auslastung** mit Farbcodierung
✅ **RAM-Status** (used/total)
✅ **CPU-Temperatur** mit Warnings
✅ **Lautstärke** + Helligkeit
✅ **Live Clock** mit Datum
✅ **Custom Widgets** erweiterbar

### Panel erweitern

```python
# In panel.py neue Widget-Klasse hinzufügen:

class CustomWidget(Gtk.Label):
    def __init__(self):
        super().__init__()
        self.update()
        GLib.timeout_add(1000, self.update)
    
    def update(self) -> bool:
        # Deine Logik
        self.set_markup(f"<span color='{COLORS['accent_cyan']}'>Data</span>")
        return True

# Dann in DojoPanelWindow.__init__:
right_box.pack_start(CustomWidget(), False, False, 0)
```

---

## 🔧 Troubleshooting

### Problem: i3 startet nicht
```bash
# Check Logs
cat ~/.xsession-errors

# Config validieren
i3 -c ~/.config/i3/config -C

# Mit Fehlerausgabe starten
i3 -V >> /tmp/i3-log.txt 2>&1
```

### Problem: Panel zeigt nicht
```bash
# GTK3 Dependencies
python3 -c "import gi; gi.require_version('Gtk', '3.0')"

# Falls fehlt:
sudo pacman -S python-gobject gtk3

# Manuell testen:
python3 ~/.config/dojo/panel.py
```

### Problem: Config-Fehler nach Update
```bash
# i3 Config validieren und neuladen
i3-msg reload
i3-msg restart

# Oder neuladen mit:
Mod+Shift+c
```

Mehr Troubleshooting → siehe `SETUP_GUIDE.md`

---

## 📚 Dokumentation

| Datei | Inhalt |
|-------|--------|
| **SETUP_GUIDE.md** | Komplette Installation (6 Phasen) |
| **SHORTCUTS.md** | Alle Keyboard Shortcuts |
| **install.sh** | Automatisierter Installer |
| **panel.py** | Custom Panel-System |
| **i3/config** | i3 Window Manager Config |

---

## 🎓 Learning Path

### Woche 1: Foundation
- [ ] DOJO installieren
- [ ] Keyboard Shortcuts lernen (SHORTCUTS.md)
- [ ] 10 häufige Workflows ausführen

### Woche 2: Customization
- [ ] i3 Config modifizieren
- [ ] Farben anpassen
- [ ] Eigene Aliases erstellen

### Woche 3: Toolkit Development
- [ ] Erstes Bash-Tool schreiben
- [ ] In DOJO integrieren
- [ ] Tastenkürzel zuweisen

### Woche 4: Advanced
- [ ] Python Security Tools
- [ ] Rust Binary Tools
- [ ] Panel Widgets erweitern

### Monats-Ziel
- Vollständig produktives Hacking-System
- 10+ eigene Tools integriert
- Personalisiert & optimiert

---

## 🚀 Deployment

Wenn alles läuft, kannst du DOJO reproduzieren:

```bash
# System-Snapshot
sudo dd if=/dev/sda of=dojo-system.img bs=4M

# Repository updaten
cd ~/dojo
git add -A
git commit -m "DOJO v1.0 - Fully configured"
git push origin main

# Auf anderen Maschinen installieren:
git clone https://github.com/dein-username/dojo.git ~/dojo
sudo ~/dojo/install.sh
```

---

## 📈 Roadmap

- [ ] v1.0: Foundation Release ✅
- [ ] v1.1: Tool Templates
- [ ] v1.2: Advanced Panel Widgets
- [ ] v2.0: CI/CD Integration
- [ ] v2.1: Custom Distro ISO

---

## 🤝 Contributing

Dieses Projekt ist **dein persönliches Trainings-Dojo**. Erweitere es:

```bash
# Branch erstellen
git checkout -b feature/my-tool

# Tool hinzufügen
~/.local/share/dojo/tools/my-awesome-tool

# Committen
git commit -m "Add: My Awesome Hacking Tool"
git push origin feature/my-tool
```

---

## 📞 Support

Bei Problemen:

```bash
# Diagnostics sammeln
journalctl -xe > /tmp/dojo-diag.txt
dmesg | tail -100 >> /tmp/dojo-diag.txt
neofetch >> /tmp/dojo-diag.txt

# i3 Config validieren
i3 -c ~/.config/i3/config -C

# Logs ansehen
tail -f ~/.xsession-errors
```

---

## 📜 Lizenz

MIT License - Du kannst DOJO verwenden, modifizieren und weitergeben

```
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```

Volltext: siehe `LICENSE`

---

## 🙏 Credits & Inspirationen

- **Arch Linux** - The OS foundation
- **i3 Window Manager** - Tiling WM excellence
- **BlackArch Linux** - Design inspiration
- **Hacker Community** - Tools & knowledge

---

## 🥋 Philosophie: Der DoJo-Weg

> *Ein Dojo ist kein Ort, an dem man perfekt wird.*
> *Es ist ein Ort, an dem man die Schranken seiner Imperfektionen erforscht.*

Dasselbe gilt für dieses Projekt:

- **Kontinuierlich lernen** - Jedes Tool ist eine Lernchance
- **Von Basics zur Meisterschaft** - Strukturierter Lernpfad
- **Experimentieren encouraged** - Modifiziere, breche, repariere
- **Sharing is caring** - Teile dein Wissen

---

## 🎯 Deine nächsten Schritte

1. **Installieren**: `sudo ./install.sh`
2. **Erkunden**: `Mod+d` → explore
3. **Customizen**: Farben & Shortcuts anpassen
4. **Bauen**: Dein erstes Tool schreiben
5. **Teilen**: Mit der Community teilen

---

```
╔═══════════════════════════════════════════════════════════════════════════╗
║                                                                           ║
║                    🥋 WILLKOMMEN IM DOJO! 🥋                            ║
║                                                                           ║
║  "The master has failed more times than the beginner has tried."        ║
║                                                          - Stephen McCranie ║
║                                                                           ║
╚═══════════════════════════════════════════════════════════════════════════╝
```

---

**Version 1.0 | Stand: 2026-01-02 | Made with ❤️ for Hackers**
