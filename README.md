# powerg-m17n

Native **m17n** input method for Amharic and Ge'ez on Linux (Fcitx5 / IBus), implementing the **Power Ge'ez Phonetic** layout.

Ported from [SIL Ethiopic Power-G](https://github.com/keymanapp/keyboards/tree/master/release/sil/sil_ethiopic_power_g) (Keyman, © SIL Ethiopia) with 100% rule parity.

---

## Installation

### 1. Prerequisites

- **Arch / Omarchy**: `sudo pacman -S m17n-db fcitx5-m17n`
- **Debian / Ubuntu**: `sudo apt install m17n-db fcitx5-m17n` _(or `ibus-m17n`)_
- **Fedora**: `sudo dnf install m17n-db fcitx5-m17n` _(or `ibus-m17n`)_

### 2. Install

```bash
git clone https://github.com/isri21/powerg-m17n.git
cd powerg-m17n
mkdir -p ~/.m17n.d
cp am-powerg.mim mdb.dir ~/.m17n.d/
```

---

## Configuration

1. **Restart your input method**:
   - **Fcitx5**: `fcitx5 -r -d`
   - **IBus**: `ibus restart`

2. **Add the keyboard**:
   - Open **Fcitx5 Configuration** (or **IBus Preferences**).
   - Uncheck **"Only Show Current Language"**, search for **Amharic**, and add `powerg (M17N)`.
   - Switch layouts using your normal shortcut.

---

## Uninstall

```bash
rm ~/.m17n.d/am-powerg.mim ~/.m17n.d/mdb.dir
```

---

## License

MIT License. Based on the SIL Ethiopic Power-G keyboard (© SIL Ethiopia).
