To get circleCI to build you have give it a v.x.x.x-leahlovise tag, and
then corresponding commit, then push the tag, and lastly push the commit

```
git commit -am v1.5.8.2-leahlovise
git tag -a v1.5.8.2-leahlovise -m 'leahlovise'
git push courihub v1.5.8.2-leahlovise
git push courihub leahlovise
```


you'll need the courihub remote in git config:

```
[remote "courihub"]
        url = git@github.com:CouriVine/reaction.git
        fetch = +refs/heads/*:refs/remotes/courihub/*
```
