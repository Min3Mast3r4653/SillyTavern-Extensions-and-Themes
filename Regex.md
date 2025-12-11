# Regex
# Regex (Regular Expression)
[Back to main list](https://github.com/Min3Mast3r4653/SillyTavern-Extensions-and-Themes) | [Cheatsheet](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions/Cheatsheet)<br>
Pattern enclosed between slashes for direct match as follows: `/abc/`<br>
To prevent `"` or `*` from being used altering the regex use `\*` or `\"`.
Using special characters for indirect matches as follows: `/ab*c/` - the `*` after `b` means `0 or more occurrences of the preceding item.` In the string `cbbabbbbcdebc`, this pattern will match the substring `abbbbc`.
## Examples
This cleans up the HTML that gets sent to help with cohesion and possibly token count.
```md
Script name: Clean HTML (From Outgoing Prompt)
Find regex: /\s?<(?!\!--)(?:"[^"]*"|'[^']*'|[^'">])*>/g
Replace with:
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
This colors **{{char}}:** without wasting tokens, this variant switches it to a slightly-dulled red in bold.
I recommend that you replace {{char}} with their actual name for scenario or multi-character cards.
```md
Script name: Colored Name
Find regex: /\**{{char}}:\**/g
Replace with: <b style="color: #FF3333;">{{char}}:</b>
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
Macros in Find Regex: Substitute (raw)
Alter Chat Display: Yes
Alter Outgoing Prompt: Yes
```
