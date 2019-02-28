# git-flow-training
Simple repository to show git flow during presentations

###### Simple flow
  1. Clone remote repository      

    https://github.com/aztor22/git-flow-training.git
	
  2. Create new branch from master
  
    git checkout -b 'features/[your_branch_name]'	

  3. Create branch on remote repository
  
    git push --set-upstream origin features/[your_branch_name]
	
  4. Add new file and commit changes
  
    git add .  
    git commit -m 'your commit msg'
	
  5. Push changes to remote branch
    git push
	
###### Flow with rebase
  1. Create new branch from master
	
    git checkout -b 'features/[your_branch_name]'
		
  2. Create branch on remote repository
	
    git push --set-upstream origin features/[your_branch_name]
		
  3. Add new file and commit changes
	
    git add .  
    git commit -m 'your commit msg'
		
  4. Ask me to do some changes and push them to master
  5. Checkout master and pull from remote
	
    git checkout master  
    git pull
		
  6. Checkout your branch and rebase changes from master
	
    git checkout features/[your_branch_name]  
    git rebase master
		
  7. Push changes to remote
	
    git push

###### Gerrit flow
  1. Create new branch from master
	
    git checkout -b 'features/[your_branch_name]'
		
  2. Create branch on remote repository
	
    git push --set-upstream origin features/[your_branch_name]
		
  3. Add new file and commit changes
	
    git add .  
    git commit -m 'your commit msg'
		
  4. Ask me to do some changes and push them to master
  5. Checkout master and pull from remote
	
    git checkout master  
    git pull
		
  6. Checkout your branch and rebase changes from master
	
    git checkout features/[your_branch_name]  
    git rebase master
		
  7. Checkout master and rebase your changes on top of master
	
    git checkout master
    git rebase features/[your_branch_name]
		
  8. Push changes to remote
	
    git push
		