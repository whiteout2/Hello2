NOTE: C:\cygwin\bin has to be on the PATH

Use: setx PATH "%PATH%;C:\cygwin\bin" 


Git remember username and password:

See: http://happygitwithr.com/credential-caching.html

11.3.1 Trigger a username / password challenge
Change a file in your local repo and commit it. Do that however you wish. Here are shell commands that will work:

echo "adding a line" >> README.md
git add -A
git commit -m "A commit from my local computer"

Now push!

git push -u origin master

One last time you will be asked for your username and password, which hopefully will be cached.

Now push AGAIN.

git push

You should NOT be asked for your username and password, instead you should see Everything up-to-date.

Rejoice and close the shell.