+++
author = "Andrew Weisbeck"
title = "Emoji Support"
date = "2025-03-05"
description = "Guide to emoji usage in Hugo"
tags = [
    "emoji",
    "hugo",
]
+++

Emoji can be enabled in a Hugo project in a number of ways.

The emojify function can be called directly in templates or Inline Shortcodes.

To enable emoji globally, set enableEmoji to true in your site's configuration and then you can type emoji shorthand codes directly in content files; e.g.

🙈 :see_no_evil: 🙉 :hear_no_evil: 🙊 :speak_no_evil:

The Emoji cheat sheet is a useful reference for emoji shorthand codes.

N.B. The above steps enable Unicode Standard emoji characters and sequences in Hugo, however the rendering of these glyphs depends on the browser and the platform. To style the emoji you can either use a third party emoji font or a font stack; e.g.

{{< highlight html >}} .emoji { font-family: Apple Color Emoji, Segoe UI Emoji, NotoColorEmoji, Segoe UI Symbol, Android Emoji, EmojiSymbols; } {{< /highlight >}}

{{< css.inline >}}
<style> .emojify { font-family: Apple Color Emoji, Segoe UI Emoji, NotoColorEmoji, Segoe UI Symbol, Android Emoji, EmojiSymbols; font-size: 2rem; vertical-align: middle; } @media screen and (max-width:650px) { .nowrap { display: block; margin: 25px 0; } } </style>

{{< /css.inline >}}
