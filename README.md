tep1: Create a repository @github    --->   git.cse.iitk.ac.in

Step2: git clone git@git.cse.iitk.ac.in:deba/classdemo.git

Step3:      $ cd classdemo
           
            $ vim README.md

            $ Add this content to README.md


Step4:
            $ git add README.md 

            $ git commit -am "adding readme"

            $ git push
                 OR 
            $ git push -u origin master   

            $ mkdir base
          
            $ cd base
     
            $ vi sample.c         /*Add a new file, create some content*/
 
            $ cd ..

            $ git add base

            $ git commit -m "adding base"
 
            $ git push    

Log:
             $ git log -p 

             $ git log --stat

             $ git log -p README.md

             $ git help log

diff:        $ git diff README.md

             $ git diff 

revert:

             $ git revert HEAD~0

             $ git commit -am "revert" 

             $ git push
           
             $ git add base/newsample.c 
            
             $ git commit -m "add newsample.c" 
              
             $ git revert HEAD~0
           
             $ git commit -am "update readme"
             
             $ git push
             
             $ git revert HEAD~1    /*Revert the revert*/
             
             $ git push

conflicts:

             Create a separate clone of the git repository

             In localA:
             
             $ git add base/newfile

             $ git commit 

             $ git push

             In localB:
             
             $ git add base/vimp.c
             
             $ git commit 

             $ git push              /*A pull required before push*/
             
             /*Modifying the same file*/

