# Regex
[Back to main list](https://github.com/Min3Mast3r4653/SillyTavern-Extensions-and-Themes) | [Cheatsheet](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions/Cheatsheet)<br>
Pattern enclosed between slashes for direct match as follows: `/abc/`<br>
Using special characters for indirect matches as follows: `/ab*c/` - the `*` after `b` means `0 or more occurrences of the preceding item.` In the string `cbbabbbbcdebc`, this pattern will match the substring `abbbbc`.

## Example
```md
Script name: Clean HTML
Find regex: /\s?<(?!\!--)(?:"[^"]*"|'[^']*'|[^'">])*>/g
Affects
- User Input: No
- AI Output: Yes
- Slash Commands: No
- World Info: No
- Reasoning: No
Min Depth: Unlimited
Max Depth: Unlimited
Disabled: No
Run On Edit: Yes
Macros in Find Regex: Don't substitute
Alter Chat Display: Yes
Alter Outgoing Prompt: Yes
```
