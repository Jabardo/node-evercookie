Process of merge exercise:

1) Go to the master branch:
	git checkout master

2) Need SHA 215ff7e of Upstream/master branch in order to merge:
	git checkout HEAD~2

3) Create aux branch to save that SHA commit of Upstream/master
	git checkout -b master_aux

4) Need SHA 7552ad9 of upstream/old branch in order to merge:
	git checkout upstream/old

5) Create stable branch to save that SHA commit of upstream/old
	git checkout -b stable

6) Merge both branches (master_aux and stable, being in stable branch)
	git merge master_aux