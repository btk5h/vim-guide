# Goto a Specific Line

Jumping to specific lines may come in handy if you're trying to fix compile-time warnings/errors.

{% tabs %}
{% tab title="Step by Step" %}
1. You must be in command-line mode. Press escape to go back to normal mode if you are in any other mode and then press `:` to enter command-line mode.
2. Type the line number you want to jump to and press enter. If you want to jump to the end of the file, use `$` instead of a line number.

#### Shortcuts for the start and end

If you only want to jump to the start of the end of the file, there are some shortcuts in normal mode that you can use to save a few keystrokes.

`gg` jumps to the start of the file

`G` jumps to the end of the file
{% endtab %}

{% tab title="Cheatsheet-Friendly" %}
Command-line commands:`:<line number>` or `:$` \(to jump to the end of the file\)

Normal mode: `gg` \(to jump the the start of the file\) or `G` \(to jump to the end of the file\)
{% endtab %}
{% endtabs %}



