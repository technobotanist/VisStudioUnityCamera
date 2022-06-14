---
layout: page
title: "Step 2: Access Your Repository"
course: "gettingstarted"
unit: 2
---
Now that you have set up your GitHub repository, we need to access it in order to make changes. Recall that there are two ways to access your instance - via the cloud and via desktop apps. You can mix and match these based on your particular needs at the time.

## Setting Up Cloud Access
Setting up cloud access for your repository is extremely easy. All you need to do is access your GitHub Repository, go to the URL in the toolbar, and change the ```.com``` to ```.dev```. For example, if your repository URL is ```https://github.com/mjsamberg/git-courseware-template/```, your edit URL is ```https://github.dev/mjsamberg/git-courseware-template/```.

Alternatively, you can click on the **Code** button, click on **Codespaces** and click **New Codespace**.

Either option will set up a new instance of Visual Studio Code in your browser that you can use to edit your site.

{% include figure.html image="start/img/codespaces.png" alt="Visual Studio Codespaces, Click Code and then Codespaces, and then New Codespace" %}

After you save changes in your Visual Studio window, click the GitHub window in the left sidebar (fourth one down, containing three circles). Click the **+** next to the **Changes** label, enter a commit message in the **Message** box (a commit messages summarizes the changes made). Click the checkbox at the top icon. When you're all done, click the **Sync Changes** button to push changes to GitHub.

{% include figure.html image="start/img/commit-vscode.png" alt="Click GitHub, Add Changes, Add Messages, click Check Box" %}

## Desktop Access
Before you proceed, you must ensure that [GitHub Desktop](https://desktop.github.com) is installed on your computer unless you are familiar with GitHub and are already using the Command Line or another tool.

To open your site in GitHub Desktop, click **Code** on the GitHub Repository website, click **Local** and click **Open with GitHub Desktop**.

{% include figure.html image="start/img/openindesktop.png" alt="To open your site in GitHub Desktop, click **Code** on the GitHub Repository website, click **Local** and click **Open with GitHub Desktop**." %}

GitHub Desktop will open and download your repository. You may be asked to sign in to GitHub the first time the app opens.

By default, if Visual Studio Code is installed, it will be the default editor. If you want to change it, open the preferences for GitHub Desktop and change the editor (to Ulysses or another editor of choice). 

Click **Open in Visual Studio Code** (or your editor) in order to open the directories in GitHub Desktop. Save your changes and then return to GitHub. Click ```Push Origin```. This will send the latest code to GitHub.com. You will do this *save, commit, push* procedure every time you want to send code to the Internet. 

### Remember: Save, Commit, Push
These are the three ingredients of getting your code into GitHub.