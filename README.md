*How to get a Discord Theme for Slack (WINDOWS)*

1. Copy-paste these into Slack: `#2f3136,#2F3136,#2F3136,#ffffff,#5a5e69,#cccccc,#43b581,#f04747`, then click on the button that says "Switch sidebar theme" under your message with the colors. 
2. Press "Windows Key + R".

3. Copy-paste this into the Run window that opens: `%homepath%\AppData\Local\slack\`, then press "Enter".

4. Open up the most recent version (e.g. app-3.3.1) then open `resources\app.asar.unpacked\src\static\`

5. Locate a file called `ssb-interop.js` and right-click it, then click "Edit".

6. Copy-paste the following into the bottom of the file, then use "CTRL + S" to save it. `document.addEventListener('DOMContentLoaded', function() {$.ajax({url: https://raw.githubusercontent.com/Art3miss/slack-discordtheme/master/black.css', success: function(css) {$("<style></style>").appendTo('head').html(css);}});});`

7. Press "CTRL + R" to restart Slack.



You're done! You now have a Discord Theme on Slack!