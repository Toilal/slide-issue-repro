---
theme: seriph
highlighter: shiki
---

# HMR issue with v-clicks and markdown list
Occurs only with v-clicks, markdown list, and items using bold/italic

---

# With markdown list
The issue occurs only when using bold or italic in items

<v-clicks>

- For some reason, **if bold is used** in the list item, changing a word won't trigger hot module reload.
- Without bold, HMR is triggered properly.
- 😭 **With bold**, it doesn't work 😭.
- 😭 **With italic**, it doesn't work either 😭.

</v-clicks>

---

# Without list
Everything works properly

<v-clicks>

**if bold is used** on a paragraph, changing a word triggers hot module reload properly.

Without bold, it works properly.

😎 **With bold**, it works 😎.

😎 **With italic**, it works too 😎.

</v-clicks>

---