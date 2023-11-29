# Git-Assignment-4
Git Commands for each step :


1.) Put master.txt on master branch, stage and commit

	mkdir git

	cd git

	git init

	touch master.txt

	git add master.txt

	git commit -m "Commiting master.txt"


2.) Create 3 branches: public1, public2 and private

	git branch public1

	git branch public2

	git branch private


3.) Put public1.txt on public 1 branch, stage and commit 

	git checkout public1.txt

	touch public1.txt

	git add public1.txt

	git commit -m "Commiting public1.txt."


4.) Merge public 1 on master branch & Merge public 2 on master branch 


	git checkout master

	git merge public1

	git merge public2


5.) Edit master.txt on private branch, stage and commit 


	git checkout private

	nano master.txt ---------> update master file by adding text in it as "Master.txt is now updated !!"

	git add master.txt

	git commit -m "Commiting updated master.txt."


6.) Now update branch public 1 and public 2 with new master code in private


	git checkout public1

	git merge private

	git checkout public2

	git merge private


7.) Also update new master code on master 

	git checkout master

	git merge private


8.) Finally update all the code on the private branch


	git checkout private

	git merge master	
