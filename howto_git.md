# Acknowledgement
This doc is based on this awesome [article](https://kbroman.org/github_tutorial/pages/init.html) by Karl Broman.
# Creating a new local repo
```
git init
```
If the repo name is master by default (depends on your local git settings) change it to `main` to
future proof:
```
git branch -m "main"
```
# Commiting changes
```
git add . && git commit -m "your commit msg"
```
# Binding to a remote repo
- first create a new repo on `github.com` manually. Make sure to create a completely *empty* repo
(not even a README);
- add a `.gitignore` file;
- then locally run (assuming ssh is configured)
```
git remote add origin git@github.com:username/new_repo
git push -u origin main
```
