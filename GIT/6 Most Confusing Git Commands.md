# 6 Most Confusing Git Commands

Understanding Git and its myriad commands can be a challenging task for many developers, especially when first introduced to it. Here, we're breaking down six of the most confusing Git commands, providing clarity on how they function:

1.  **`git merge`**:
    
    -   This command is used to combine multiple sequences of commits into one unified history.
    -   The visual representation shows two diverging commit sequences. After the `git merge`, they're combined, resulting in a "Post Merge" sequence.
2.  **`git rebase`**:
    
    -   Rebase is a way to integrate changes from one branch into another.
    -   It involves moving the entire sequence of commit history onto a new base commit.
    -   The representation showcases a sequence of commits being rebased, leading to a "Post Rebase" sequence.
3.  **`git reset`**:
    
    -   This command is used to undo changes in your working directory.
    -   The visualization displays a sequence of commits. After executing `git reset`, a portion of the commit sequence is removed, resulting in a "Post Reset" sequence.
4.  **`git revert`**:
    
    -   The `git revert` command undoes a committed snapshot but, instead of deleting the commit, it creates a new commit that undoes all the changes.
    -   The illustration presents a sequence of commits. After a `git revert`, a new commit is added to reverse the changes of a previous commit, leading to a "Post Revert" sequence.
5.  **`git fetch`**:
    
    -   This command is used to retrieve updates from a remote repository.
    -   The diagram depicts the flow from the "remote origin/main" to the local "main". It fetches the changes but doesn't merge them.
6.  **`git pull`**:
    
    -   A `git pull` is essentially a `git fetch` followed by a `git merge`.
    -   It retrieves updates from a remote repository and then merges them into the current branch in the local repository.
    -   The representation indicates the flow from the "remote origin/main" to the local "main", highlighting both fetching and merging processes.

Simplified and concise illustration of commands for better understanding

𝟭. 𝗴𝗶𝘁  𝗺𝗲𝗿𝗴𝗲  𝘃𝘀  𝗴𝗶𝘁  𝗿𝗲𝗯𝗮𝘀𝗲:

- 𝘨𝘪𝘵 𝘮𝘦𝘳𝘨𝘦 combines branch changes with new merge commits

- 𝘨𝘪𝘵 𝘳𝘦𝘣𝘢𝘴𝘦 moves branch changes on top, creating a linear history

  

𝟮. 𝗴𝗶𝘁  𝗿𝗲𝘀𝗲𝘁  𝘃𝘀  𝗴𝗶𝘁  𝗿𝗲𝘃𝗲𝗿𝘁:

- 𝘨𝘪𝘵 𝘳𝘦𝘴𝘦𝘵 undoes changes and moves the branch pointer, discarding subsequent commits

- 𝘨𝘪𝘵 𝘳𝘦𝘷𝘦𝘳𝘵 creates new undo commits, preserving history

  

𝟯. 𝗴𝗶𝘁  𝗳𝗲𝘁𝗰𝗵  𝘃𝘀  𝗴𝗶𝘁  𝗽𝘂𝗹𝗹:

- 𝘨𝘪𝘵 𝘧𝘦𝘵𝘤𝘩 downloads remote changes without auto-merging

- 𝘨𝘪𝘵 𝘱𝘶𝘭𝘭 fetches and auto-merges remote changes

In short,

git pull = git fetch + git merge

<p></p>
<p>
  <img src="../images/git/git1.png" style="width: 640px">
</p>