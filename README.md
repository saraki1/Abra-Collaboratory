# Abra-Collaboratory
This repository contains more than just code, it provides a framework for reproducible research and collaboration in the form of a detailed and transparent narrative of a project's research process. For detailed information on how we use GitHub as a reproducible research platform, click [here](https://github.com/callahantiff/Abra-Collaboratory/wiki/Using-GitHub-as-a-Reproducible-Research-Platform).

<img src="https://img.shields.io/badge/ReproducibleResearch-AbraCollaboratory-magenta.svg?style=plastic" alt="git-AbraCollaboratory">

<br>

## Getting Started  
Please note that we are working on automating the process of settting up a new reproducible reserach project. In the meantime, follow the instructions below.

To get started, please follow the steps listed below:
* [Fork the Project Repository](#fork-the-project-repository)
* [Fork the Project Wiki](#fork-the-project-wiki)
* [Add Projects Boards](#add-projects-boards)
* [Invite Collaborators](#invite-collaborators)


### Fork the Project Repository
- Open a terminal and create a local clone of the repository
```bash
$ git clone https://github.com/callahantiff/Abra-Collaboratory.git
Cloning into 'Abra-Collaboratory'...
remote: Enumerating objects: 91, done.
remote: Counting objects: 100% (91/91), done.
remote: Compressing objects: 100% (74/74), done.
remote: Total 91 (delta 15), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (91/91), done.
```

- Create a new repository in your GitHub profile and name it "Abra-Collaboratory"
```bash
$ curl -u 'username' https://api.github.com/user/repos -d '{"name":"Abra-Collaboratory"}'
```

- Change directories to the "Abra-Collaboratory" repository you just cloned and update the origin branch to the url for the new GitHub project you just created. That's it! Before moving onto the next step, verify that you have the same files in your new repository that are in the original "Abra-Collaboratory" project.
```bash
$ cd Abra-Collaboratory
$ git remote rm origin
$ git remote add origin https://github.com/{username}/Abra-Collaboratory.git
$ git push -u origin master
```

<br>

### Fork the Project Wiki
- Fork the wiki into your local "Abra-Collaboratory" directory.

```bash
$ git clone https://github.com/callahantiff/Abra-Collaboratory.wiki.git
Cloning into 'Abra-Collaboratory.wiki'...
remote: Enumerating objects: 47, done.
remote: Counting objects: 100% (47/47), done.
remote: Compressing objects: 100% (45/45), done.
remote: Total 47 (delta 20), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (47/47), done.
```

- Then, go to Wiki [here](https://github.com/username/Abra-Collaboratory/wiki) and create an empty homepage (example shown below):
<img src="https://github.com/callahantiff/Abra-Collaboratory/blob/master/resources/documentation/images/wiki/wiki_clone.png">

- Once you have crated the wiki page, complete the final steps, in the order shown below.
```bash
$ cd Abra-Collaboratory.wiki
$ git fetch
$ git remote add wiki-fork https://github.com/{username}/Abra-Collaboratory.wiki.git
$ git push wiki-fork -f
Counting objects: 93, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (76/76), done.
Writing objects: 100% (93/93), 6.46 MiB | 1.82 MiB/s, done.
Total 93 (delta 16), reused 0 (delta 0)
remote: Resolving deltas: 100% (16/16), done.
To https://github.com/{user}/Abra-Collaboratory.wiki.git
 + 4bba267...599d6ec master -> master (forced update)
```

<br>

### Add Projects Boards 
Unfortunately, there is not yet a way to clone GitHub Projects boards. That being said, there is still a way that you can access this information and add it to your rerpository. In order to do this, complete the following steps (as shown in the screenshot below):
  1. Go to the "Abra-Collaboratory" [Projects boards](https://github.com/callahantiff/Abra-Collaboratory/projects)
  2. Click and open each board and navigate to the "Menu" as shown below
  3. Inside the "Menu", click on "Copy"
  4. Select the dropdown and find your "{username}/Abra-Collaboratory"
  5. Verify the checkbox to include "Automation settings" is checked
  6. Remove "[COPY]" from the Project board name textbox

Once you have performed these steps, push the green button and copy the copy. Repeat these steps for each of the four "Abra-Collaboratory" Projects boards.

<img src="https://github.com/callahantiff/Abra-Collaboratory/blob/master/resources/documentation/images/wiki/git_projects.png">

<br>

- [x] **Verify Issue Templates Transfer** 
If you correctly cloned the "Abra-Collaboratory" repository, you should see the follow documents in your project homepage:

<img src="https://github.com/callahantiff/Abra-Collaboratory/blob/master/resources/documentation/images/wiki/cloned_repo.png">

***

<br>

### Invite Collaborators
Now that you have cloned the repository, wiki, have copied the project boards, and verified the issue templates, you are ready to customize the repo for your project. At this point we recommend that you update the README and Wiki homepage to describe your project.

You are now ready to invite your collaborators! To make this process easier, we have written a template email, which you will find [here](https://github.com/callahantiff/Abra-Collaboratory/blob/master/resources/New_Collaborators_Invitation_Email.md). To use this template, update the slots denoted with "{}" and navigate to the "Preview Button". At that point, you should see something similar to the image shown below. From the "Preview", copy and paste the text directly into an email.

<img src="https://github.com/callahantiff/Abra-Collaboratory/blob/master/resources/documentation/images/wiki/collaborator-email.png">
