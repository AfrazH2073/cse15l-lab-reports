
4. Log into ieng6 account 
`<up> <up> <enter>`
<img width="563" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/b93e39b7-c4dd-48fa-ad21-54b2c344aeeb">

Here we are logging into ieng6 account, and I am using up arrow keys to access old commands that I typed before. I accessed the command from my terminal history by repeatedly typing the up arrow key to access my earlier instance of running the ` ssh cs15lfa23eg@ieng6.ucsd.edu `



5. Clone your fork of the repository from your Github account (using the SSH URL)
` <up> <up> <up> <up> <up> <up> <enter>  `

<img width="570" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/a58d1ad9-06bd-4460-896e-cf0469ccd34d">

Here, I am cloning the git repository, in order to access the code in my machine, also known as git cloning it, and I do it by hitting the up arrow key several times to access my earlier clone message I did during the lab, using my terminal history.

6. Run the tests, demonstrating that they fail
`c d <space> l <tab> <enter>  b a s h <space> t <tab> <enter>`

Here I CD into lab7 first in order to access the file to run for the tests by being in the same directory, and then I used bash test.sh in order to run the .sh file and run the tests, I used <tab> to autofill the command, and ran it in the terminal.

<img width="619" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/504677b6-35b6-4577-b239-df942cce2910">


8. Edit the code file to fix the failing test
` vim <shift> L <tab> . <tab> 43 j e r 2 <shift> : w q <enter> `

Here I run VIM in order to edit and fix the bug in ListExamples.java, navigating to the bug and fixing index1 to be index2 in the screenshot, and saving it using ` :wq ` .

<img width="401" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/d3b6e8fe-39c7-410b-b5de-31c2a30281d9">


<img width="379" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/62e6d00b-b9e0-4c13-9567-d50f221e3b42">

9. Run the tests displaying that they succeed.

` b a s h <space> t <tab> <enter> `

Here I run the same ` bash test.sh ` test I did before, but this time the tests demonstrate success since I fixed the bug, and I used <tab> to autofill the rest of the command.

  <img width="478" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/5b99c269-b267-43cf-80e2-7d8a5c40e798">


11. Commit and push the resulting change to your Github account (you can pick any commit message!)
`<up> <up> <up> <up> <up> g i t <space> c o m m i t <space> - m <space> " c o m m i t " <enter> g i t <space> p u s h <enter> `

Here, I use `git commit `to commit and publish changes locally  and giving it a message of "commit" and then using `git push` to push my changes to the repository to update for all users accessing the github.

<img width="592" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/3800ccf3-1883-4c9b-8577-904490201d33">



