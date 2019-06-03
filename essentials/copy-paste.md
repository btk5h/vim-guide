# Copy/Paste

{% tabs %}
{% tab title="Step by Step" %}
1. You must be in normal mode. Press escape to go back to normal mode if you are in any other mode.
2. Move your cursor to the start or end of the text you want to copy.
3. Press `v` to enter selection mode. If you want to select entire lines, you can use `V` instead.
4. Move your cursor so that the entire block of text you want to select is highlighted.
5. Press `y` to copy \("yank"\). If you want to copy and delete the selected text, you can use `d` instead.
6. You are now in normal mode, navigate your cursor to the location where you want to paste.
7. Press `p` to paste the text after your cursor. If you want to paste the text before your cursor, you can use `P` instead.
{% endtab %}

{% tab title="Cheatsheet-Friendly" %}
Entering visual mode: `v` \(to select character-by-character\) or `V` \(to select line-by-line\)  
In visual mode: `y` \(copy or "yank"\) or `d` \(copy and delete\)  
In normal mode: `p` or `P`
{% endtab %}
{% endtabs %}

{% hint style="warning" %}
#### I can't paste the text I copied in vim into other programs!

The text you copy in vim is stored in a location separate from the system clipboard. Unfortunately there are no \(convenient\) shortcuts that will allow you to access the system clipboard.
{% endhint %}



