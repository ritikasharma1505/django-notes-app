# Simple Django CI/CD Project 
This is a simple notes app built with React and Django.
This repo is not cloned locally.. this project is remotely available


![pipeline-config](https://github.com/user-attachments/assets/c24e7c69-0d94-4695-8960-a98ca54ca338)

![Jenkinsfile-from-SCM](https://github.com/user-attachments/assets/15bbbf0f-fe9c-4547-aa00-cbd359f22988)

![DjangoCICD-auto-buildtrigger-github-webhooks-integration](https://github.com/user-attachments/assets/8750666f-eadb-4dfd-ac67-e842ad0b41c5)


![github-hook-log-on-jenkins](https://github.com/user-attachments/assets/f2479108-7de5-4af6-a626-cedca7eecf03)

![DjangoCICD-auto-buildtrigger-github-webhooks-integration-final](https://github.com/user-attachments/assets/68ec92a4-e68b-4fe6-ba08-54d1771c8761)


Troubleshooting steps :
This was hard until GitHub hooks came into the picture, make sure the same git repo is used in Jenkinsfile for which you created GitHub webhooks(which means fork the project), I mistakenly used the instructor's, and the auto build trigger wasn't working

