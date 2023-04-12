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
<h3>Git Add All<h3>
<p>We can add more than one files in Git, but we have to run add command repeatedly.Git facilitates us with a unique option of the add command by which we can add all the available files at once.To add all the files from the repository,run the add command with <b>-A</b> option.We can use '.' instead of <b>-A</b> option.This command will stage all the files at a time.</p>
<code><pre>git add -A</pre></code>
        <code><pre>git add .</pre></code>
        <p>Consider the below output:</p>
<img src="sample images/output.png" width="450">
 <p>In the above output, all the files are displaying as untracked files by Git. To track all of these files at once, run the below command:</p>
 <code><pre>git add -A</pre></code>
 <img src="sample images/addall.png" width=450">
 <p>In the above output, all the files have been added. The status of all files is displaying as staged.</p>




