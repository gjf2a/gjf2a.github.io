---
layout: default
---

# How to privately clone a GitHub repository

These instructions are adapted from [Harry Wang](https://harrywang.me/private-repo).

1. Clone the original repository locally:
```
git clone https://github.com/gjf2a/csci335 my-csci335
```

2. Remove connection to the original repository:
```
cd my-csci335
git remote remove origin
```

3. Go to GitHub and select the option to create new private repository:<br>
<img src="../assets/images/new-repo-dropdown.png">

4. When creating the new private repository, mark it as private:<br>
<img src="../assets/images/new-repo-private.png">

5. Add your new private repository as the remote for your clone. (Of course, you won't be using the `gjf2a` account - substitute your own userid in
place of `gjf2a`):
```
git remote add origin https://github.com/gjf2a/my-csci335
```

6. Push the cloned code to your private repository:
```
git push -u origin main
```

If the above doesn't work, try this instead:
```
git push -u origin master
```
