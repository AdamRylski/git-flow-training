# git-flow-training
Simple repository to show git flow during presentations

Tutorial steps:
1. Simple flow
	* Clone remote repository
        
		https://github.com/aztor22/git-flow-training.git
		
	* Create new branch from master
	
        git checkout -b 'features/[your_branch_name]'
		
	* Create branch on remote repository
	
        git push --set-upstream origin features/[your_branch_name]
		
	* Add new file and commit changes
	
        git add .
        git commit -m 'your commit msg'
		
	* Push changes to remote branch
	
        git push
        
		
Always pull master from remote before starting next steps

2. Flow with rebase
	* Create new branch from master
	
        git checkout -b 'features/[your_branch_name]'
		
	* Create branch on remote repository
	
        git push --set-upstream origin features/[your_branch_name]
		
	* Add new file and commit changes
	
        git add .
        git commit -m 'your commit msg'
		
	* Ask me to do some changes and push them to master
	* Checkout master and pull from remote
	
        git checkout master
        git pull
		
	* Checkout your branch and rebase changes from master
	
        git checkout features/[your_branch_name]
        git rebase master
		
	* Push changes to remote
	
        git push


3. Gerrit flow
	* Create new branch from master
	
        git checkout -b 'features/[your_branch_name]'
		
	* Create branch on remote repository
	
        git push --set-upstream origin features/[your_branch_name]
		
	* Add new file and commit changes
	
        git add .
        git commit -m 'your commit msg'
		
	* Ask me to do some changes and push them to master
	* Checkout master and pull from remote
	
        git checkout master
        git pull
		
	* Checkout your branch and rebase changes from master
	
        git checkout features/[your_branch_name]
        git rebase master
		
	* Checkout master and rebase your changes on top of master
	
        git checkout master
        git rebase features/[your_branch_name]
		
	* Push changes to remote
	
        git push
		