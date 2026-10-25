# bepocyr

A keyboard layout for writing Russian, based on the bépo layout (phonetically).

## Installation (for Ubuntu 26.04, and probably other newer distributions)

1. Copy the `bepocyr` file to `~/.config/xkb/symbols/`.
2. Copy the `evdev.xml` file to `~/.config/xkb/rules/`.
3. You may have to run `gsettings set org.gnome.desktop.input-sources show-all-sources true`
4. Add the new layout in the settings.
5. Log out and log in again.

## Installation (for Ubuntu 24.04, probably works on other older distributions)

1. Copy the `bepocyr` file to `/usr/share/X11/xkb/symbols/bepocyr`.
2. Edit the `/usr/share/X11/xkb/rules/evdev.xml`, adding the following layout next
   to an existing one:
```
    <layout>
      <configItem>
        <name>bepocyr</name>
        <shortDescription>ru</shortDescription>
        <description>Cyrillic (phonetic, bepo)</description>
        <languageList>
          <iso639Id>rus</iso639Id>
        </languageList>
      </configItem>
    </layout>
```
3. Add the new layout in the settings.
4. Log out and log in again.
