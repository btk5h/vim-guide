# Find/Replace

## Find \(without replacing\)

{% tabs %}
{% tab title="Step by Step" %}
1. You must be in normal mode. Press escape to go back to normal mode if you are in any other mode.
2. Press `/`. Your cursor will move to the bottom of the screen.
3. Type the text you want to search for and hit enter. Your cursor will jump to the next occurrence of that text.
4. If you want to jump to the next occurrence of that text again, just press `n` \(for **n**ext\) in normal mode.
{% endtab %}

{% tab title="Cheatsheet-Friendly" %}
In normal mode:  
`/<text to search>` search  
`n` jump to the **n**ext occurrence
{% endtab %}
{% endtabs %}

## Find and Replace

{% tabs %}
{% tab title="Step by Step" %}
1. You must be in command-line mode. Press escape to go back to normal mode if you are in any other mode and then press `:` to enter command-line mode.
2. Enter a command in the format  `%s/<text to find>/<text to replace>/g`

#### Breakdown of the find and replace command

`%` tells vim that you want to execute the command on every single line of the file. Without this, you would only perform the operation on the current line.

`s` means "substitute"

`/<text to find>/<text to replace>/` is the find and replace operation you want to perform. Occurrences of `<text to find>` will be replaced with `<text to replace>`

`g` means "global", meaning every single occurrence in a single line will be replaced. Without this, if you had multiple occurrences of `<text to find>` on a single line, only the first one would be replaced.
{% endtab %}

{% tab title="Cheatsheet-Friendly" %}
Command-line commands: `%s/<text to find>/<text to replace>/g`
{% endtab %}
{% endtabs %}

