steps to fork
Step 1: Set up Git
If you haven't yet, you should first set up Git. Don't forget to set up authentication to GitHub from Git as well.

Step 2: Create a local clone of your fork
Right now, you have a fork of the Spoon-Knife repository, but you don't have the files in that repository on your computer. Let's create a clone of your fork locally on your computer.

On GitHub, navigate to your fork of the Spoon-Knife repository.

Above the list of files, click  Code.

"Code" button
To clone the repository using HTTPS, under "Clone with HTTPS", click . To clone the repository using an SSH key, including a certificate issued by your organization's SSH certificate authority, click Use SSH, then click .

The clipboard icon for copying the URL to clone a repository
Open Git Bash.

Change the current working directory to the location where you want the cloned directory.

Type git clone, and then paste the URL you copied earlier. It will look like this, with your GitHub username instead of YOUR-USERNAME:

$ git clone https://github.com/YOUR-USERNAME/Spoon-Knife
Press Enter. Your local clone will be created.

$ git clone https://github.com/YOUR-USERNAME/Spoon-Knife
> Cloning into `Spoon-Knife`...
> remote: Counting objects: 10, done.
> remote: Compressing objects: 100% (8/8), done.
> remove: Total 10 (delta 1), reused 10 (delta 1)
> Unpacking objects: 100% (10/10), done.
Now, you have a local copy of your fork of the Spoon-Knife repository.

Step 3: Configure Git to sync your fork with the original Spoon-Knife repository
When you fork a project in order to propose changes to the original repository, you can configure Git to pull changes from the original, or upstream, repository into the local clone of your fork.

On GitHub, navigate to the octocat/Spoon-Knife repository.

Above the list of files, click  Code.

"Code" button
To clone the repository using HTTPS, under "Clone with HTTPS", click . To clone the repository using an SSH key, including a certificate issued by your organization's SSH certificate authority, click Use SSH, then click .

The clipboard icon for copying the URL to clone a repository
Open Git Bash.

Change directories to the location of the fork you cloned in Step 2: Create a local clone of your fork.

To go to your home directory, type just cd with no other text.
To list the files and folders in your current directory, type ls.
To go into one of your listed directories, type cd your_listed_directory.
To go up one directory, type cd ...
Type git remote -v and press Enter. You'll see the current configured remote repository for your fork.

$ git remote -v
> origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
> origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
Type git remote add upstream, and then paste the URL you copied in Step 2 and press Enter. It will look like this:

$ git remote add upstream https://github.com/octocat/Spoon-Knife.git
To verify the new upstream repository you've specified for your fork, type git remote -v again. You should see the URL for your fork as origin, and the URL for the original repository as upstream.

$ git remote -v
> origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
> origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
> upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (fetch)
> upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (push)
Now, you can keep your fork synced with the upstream repository with a few Git commands. For more information, see "Syncing a fork."

