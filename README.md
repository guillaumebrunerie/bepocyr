# bepocyr

A keyboard layout for writing Russian, based on the bépo layout (phonetically).

## Installation (for Ubuntu at least, probably works on other distributions)

1. Copy the `bepocyr` file to `/usr/share/X11/xkb/symbols/bepocyr`.
2. Edit the /usr/share/X11/xkb/rules/evdev.xml, adding the following layout next
   to an existing one:

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

3. Add the new layout in the settings.
4. Log out and log in again.
