# git-tutorial
<p><ul><li>Git is a version control system.</li>
        <li>Git helps to keep track of code changes.</li>
        <li>Git is used to collaborate on code.</li></ul></p>
<p>In this tutorial,we will learn Git commands.</p>
<p>The first thing we need to do, is to check if Git is properly installed:</p>
<code><pre>git --version</pre></code>
<img src="sample images/version.png" width="450">
<h3>Configure Git</h3>
<p>Now let Git know who you are.</p>
<code><pre>git config --global user.name "your username"
git config --global user.email "your email"</pre></code>     
<img src="sample images/configure.png" width="450">
<h3>Creating Git Folder</h3>
<p>Now lets's create a new folder for our project.</p>
<code><pre>mkdir myproject
cd myproject</pre></code>
<img src="sample images/folder.png" width="450">
<p>mkdir makes a new directory.</p>
<p>cd changes the current working directory.</p>
<h3>Git Init</h3>
<p>Once you have navigated to the correct folder, you can initialize Git on that folder</p>
<code><pre>git init</pre></code>
<img src="sample images/init.png" width="450">
<p>You just created your first git Repository!</p>
<h3>Git Add</h3>
<p>You just created your first local Git repo.But it is empty.</p>
<p>So let's add some files, or create a new file using your favourite text editor. Then save or move it to the folder you just created.</p>
<p>The git add command is used to add file contents to the Index(Staging area)</p>
<code><pre>git add index.html</pre></code>
<img src="sample images/add.png" width="450">
<h3>Git Status</h3>
<p>The git status command show modified files in working directory, staged for your next commit.Staged files are files that are ready to be committed to the repository you are working on.</p>
<code><pre>git status</pre></code>
<img src="sample images/status.png" width="450">
<p>Now the file has been added to the staging environment.</p>
<h3>Git Add All</h3>
<p>We can add more than one files in Git, but we have to run add command repeatedly.Git facilitates us with a unique option of the add command by which we can add all the available files at once.To add all the files from the repository,run the add command with <b>-A</b> option.We can use '.' instead of <b>-A</b> option.This command will stage all the files at a time.</p>
<code><pre>git add -A</pre></code>
        <code><pre>git add .</pre></code>
        <p>Consider the below output:</p>
<img src="sample images/output.png" width="450">
 <p>In the above output, all the files are displaying as untracked files by Git. To track all of these files at once, run the below command:</p>
 <code><pre>git add -A</pre></code>
 <img src="sample images/addall.png" width=450">
 <p>In the above output, all the files have been added. The status of all files is displaying as staged.</p>
 <h3>Git Reset</h3>
 <p>We can undo a git add operation.We can do it through git reset command.</p>
 <code><pre>git reset <filename></pre></code>
 <img src="sample images/reset.png" width="450">
 <h3>Git Commit</h3>
 <p>The git commit command is used to record the changes in the reposiory.Git considers each commit change point or save point.It is a point in the project where you can go back to if you find a bug,or want to make a change.When we commit, we should always include a message.</p>
 <code><pre>git commit -m "Commit message"</pre></code>
 <img src="sample images/commit.png" width="450">
 <p>The Staging Environment has been committed to our repo, with the message: "First commit".</p>
 <h3>Git Clone</h3>
 <p>The git clone command is used to make a loacal copy of a remote repository.It accesses he repositry through a remote URL.</p>
 <code><pre>git clone <repository URL></pre></code>
 <img src="sample images/clone.png" width="450">
 <h3>Git Branch</h3>
 <p>A branch is a version of repository that diverges from the main working project.A Git project can have more than one branch. These branches are a pointer to a snapshot of your changes. </p>
 <p>The git branch command is used to create a new branch.</p>
 <code><pre>git branch <branch name></pre></code>
 <img src= "sample images/branch.png" width="450">
 <p>You can list all of the available branches in your repostory by using the following command.</p>
 <code><pre>git branch --list</pre></code>
 <p><b>or</b></p>
 <code><pre>git branch</pre></code>
 <img src="sample images/branchlist.png" width="450">
 <p>You can delete the specified branch.Below is the command to do this.</p>
 <code><pre>git branch -d <branch name></pre></code>
 <img src="sample images/delete.png" width="450">
 <h3>Git checkout</h3>
 <p>The git checkout command is used to switch between the branches without making a commit.</p>
 <code><pre>git checkout <branch name></pre></code>
 <img src="sample images/checkout.png" width="450">
 <h3>Git Merge</h3>
 <p>The git merge command allow you to merge the other branch with the currently active branch.</p>
 <code><pre>git merge <branch name></pre></code>
 <img src="sample images/merge.png" width="450">
<h3>Git Fetch</h3>
<p>We can fetch the complete repository with the help of fetch command from a repository URL.</p>
<code><pre>git fetch repository Url</pre></code>
<img src="sample images/fetch.png" width="450">
<p>In the above output, the complete repository has fetched from a remote URL.</p>
<h3>Git Pull</h3>
<p>The term pull is used to receive data from Github.It fetches and merges changes from the remote repository to local repository.The git pull is a combination of two commands, git fetch followed by git merge.</p>
<code><pre>git pull remote branch URL</pre></code>
<img src="sample images/pull.png" width="450">
<p>There is another way to pull the repository. We can pull the repository by using the git pull command.</p>
<code><pre>git pull options remotebranchname
git pull origin master  </pre></code>
<img src="sample images/pullorigin" width="450">
<p>In the above syntax, the term origin stands for the repository location where the remote repository situated. Master is considered as the main branch of the project.</p>
<h3>Git Push</h3>
<p>The push term refers to upload local repository content to a remote repository. Pushing is an act of transfer commits from your local repository to a remote repository</p>
<code><pre> git push option [Remote URL branch name refspec...]</pre></code>
<img src="sample images/push.png" width="450">
<p>git push origin master pushed the local content on the master branch of the remote location.</p>
<h3>Git Log</h3>
<p>Git log command is one of the most useful commands of git.Every time you need to check the history,you have to use the git log command.The basic git log command will display the most recent commits and the status of the head</p>
<code><pre>git log</pre></code>
<img src="sample images/log.png" width="450">
<h3>Git Rm</h3>
<p>In Git, the term rm stands for remove.The key function of git rm is to remove tracked files from the Git index. Additionally, it can be used to remove files from both the working directory and staging index.</p>
<code><pre>git rm file Name</pre></code>
<img src="sample images/remove.png" width="450">





