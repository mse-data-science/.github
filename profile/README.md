# 🚀 MSE Data Science @ FHNW

Welcome to **MSE Data Science**, a student-led GitHub organization by two curious minds pursuing the **Master of Engineering (MSE) in Data Science** at **FHNW – University of Applied Sciences and Arts Northwestern Switzerland** 🇨🇭.

This org is our digital lab: a place where coursework meets curiosity, theory meets practice, and ideas turn into code.

## 👥 Participants

| Name                 | GitHub                               |
| -------------------- | ------------------------------------ |
| **Si Ben Tran**      | [@7ben18](https://github.com/7ben18) |
| **Aaron Brülisauer** | [@Nodøn](https://github.com/nod0n)   |

## Important Links

- [Dates academic year](https://moodle.msengineering.ch/mod/folder/view.php?id=7936)
- [Timetables](https://moodle.msengineering.ch/mod/folder/view.php?id=7934)
- [Venues](https://moodle.msengineering.ch/mod/folder/view.php?id=12249)

## Config and Commands

### Git Config

``` bash
git config --global fetch.prune true
git config --global merge.conflictStyle zdiff3
git config --global rerere.enabled true
git config --global pack.usezstd true
git config --global pack.compression 9
git config --global core.compression 9
```

### Update all Repos

```bash
cd path_to_my_gh_org  # replace with your path
set -euo pipefail  # do not continue on failure!
for r in * .github; do
    [ -d "$r/.git" ] || continue  # skip if not git repo
    (cd "$r" && git pull --all --prune)  # in subshell: cd && pull
done
```
