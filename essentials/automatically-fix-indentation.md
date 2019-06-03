# Automatically Fix Indentation

You may find the need to fix the indentation of code that you're working on. Instead of manually going to each line and changing the indentation, vim has a shortcut that can automatically format the entire file

{% tabs %}
{% tab title="Step by Step" %}
1. You must be in normal mode. Press escape to go back to normal mode if you are in any other mode.
2. Type `gg` \(Capitalization matters! These must be lowercase g's.\) Your cursor should jump to the top of the file.
3. Type `=G` \(Capitalization matters here, too.\) The `=` tells vim to start indenting lines from your cursor and the `G` tells vim to stop indenting lines until the end of the file.
{% endtab %}

{% tab title="Cheatsheet-Friendly" %}
In normal mode: `gg=G`
{% endtab %}
{% endtabs %}

