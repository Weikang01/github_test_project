**This is a demo project for Github testing purpose**

The following instructions are made based on the video of [Ako Dev](https://www.youtube.com/channel/UCI2-MCj7pV0i0vxtl2NqZzg): [How to use GIT when working with a team? - YouTube](https://www.youtube.com/watch?v=jhtbhSpV5YA)

1. Clone the project to your local hard disk

```bash
git clone https://github.com/Weikang01/github_test_project.git
```

2. Create a new branch

```bash
git checkout -b update_text
```

3. Make modifications
4. Check Git status

```bash
git status
```

5. Add files to the commit

```bash
git add -A
```

6. Commit files with message

```bash
git commit -m "updated the text"
```

7. Upload the branch to Git

```bash
git push -u origin update_text
```

8. Update the newest version of the project from origin/master

   > Do this after uploaded your branch in order to prevent merge conflict

```bash
git pull origin master
```

9. Go back to the local master branch, update the local master, and delete (locally) the temporary branch

```bash
git checkout master
git pull
git branch -D update_text
```

## How to solve merge conflict

8. When updating the newest version of the project from origin/master, there is a merge conflict message shows in the console

```bash
git pull origin master
```

```console
CONFLICT (content): Merge conflict in *.*
Automatic merge failed: fix conflicts and then commit the result
```

9. Go to your code editor and select the code you want to keep

10. **SAVE** the files which reported merge conflict
11. add and commit

```bash
git add -A
git commit -m "merge conflict resolved"
```

12. Push the local version to Git

```bash
git push
```

13. return to master branch and delete the temporary branch

```bash
git checkout master
git pull
git branch -D update_text
```

> **TIPS: Always Remember to Pull from master to keep your code up to date**