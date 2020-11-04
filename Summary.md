# Summary of Git Practice


## Part I: About Branches

- #### Fetch a remote branch and merge it into local current working branch 
  `git pull <remote> <remote branch>`

- #### Fetch a remote branch and merge it into both current working branch and local specified branch
  `git pull <remote> <remote branch>:<local spcified branch>`

- #### Push a local branch to remote branch in regardless of what the current working branch is
  `git push <remote> <local branch>:<remote branch>`

  > ### Note
  > The notation ':' means '->',that is,'a:b' means 'a->b',which is from a to b.     
 
- #### CRUD remote branches
  _Create_     
  No need to create a remote branch before push.Just push a local branch to a remote branch which is you want to create.     
  `git push <remote> <existing local branch>:<the remote branch you try to create>`  
         
  _Delete_    
  Use `git push` command instead of `git branch` command.   
  `git push <remote> --delete <the remote branch you want to delete>`      
  
  _Read_    
  `git branch -a`    
  
  _Update_     
  There isn't a way to directly rename a Git branch in a remote repository.You will need to delete the old branch,then push a branch with the name you want to the remote repository. 
  
- #### CRUD local branches
  _Create_   
  Create and checkout a new branch.     
  `//one way`   
  `git checkout -b <new branch>`    
  
  `//another way`     
  `git branch <new branch>`  
  `git checkout <new branch>`    
  
  _Delete_   
  The working branch(current branch) can't be the branch to be deleted.  
  `git branch -d/D <branch to be deleted>`  
  
  _Read_    
  `git branch -a`    
  
  _Update_    
  Move/rename a branch.   
  `git branch -m <new name>`  
 
 




