# What happens when you initialize a repository? Why do you need to do it?
    System gonna create a `.git` folder, this process called "git initialize", this change the regular folder to git repository

# How is the staging area different from the working directory and the repository? What value do you think it offers?
    Repository contains a bunch of commits and staging area contains files prompted from working directory, whcich eventually become commit.
# How can you use the staging area to make sure you have one commit per logical change?
    `git diff` compare working directory with staging area, `git diff --staged` compare staging area with last commit, `git diff commitID1 commitID2`
    compare with `commitid1` with `commitid2`

# What are some situations when branches would be helpful in keeping your history organized? How would branches help?
    when you want to add some experiment features, add different languages, try some thing new, it's better not to interrupt the history you programmed.

# How do the diagrams help you visualize the branch structure?
    We can use `git log --graph --online` to find each commit's parents and find out which commit is not reachable, figure out what `deatched HEAD` situation is.

# What is the result of merging two branches together? Why do we represent it in the diagram the way we do?
    Some change gonna preserve, some gonna delete, it depends one the parent commit.

# What are the pros and cons of Git’s automatic merging vs. always doing merges manually?
    The pros is it easy for us, we don't bohter what happend under the hood, but the cons is git are not so smart to figure out what conflict might be, so we have
    to merge it manually.
