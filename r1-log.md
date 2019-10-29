# #100DaysOfCode Log - Round 1 - [Your Name Here]

The log of my #100DaysOfCode challenge. Started on [July 17, Monday, 2017].

## Log

### Day 1: 20191001, Tue

**Today's Progress**: Forked the [100DaysOfCode project](https://www.100daysofcode.com/). Updates will be made to this log from sourcetree. 
Goal is to get some working python code that can make REST API calls to complete simple tasks on BIG-IP, BIG-IQ, and in multiple environments like AWS, GCP, Azure, etc. 

Method is to use an existing linuxacademy account for some training vids

[Introduction to Python Development](https://linuxacademy.com/cp/modules/view/id/311)

[Programming Use Cases with Python](https://linuxacademy.com/cp/modules/view/id/383)

[Python 3 Scripting for System Administrators](https://linuxacademy.com/cp/modules/view/id/168)

, [talkpython repo ](https://github.com/talkpython/100daysofcode-with-python-course) to get ideas on topics to cover, and also spend time working on my REST API code. 

Built lab using altinstall

```
# python3.7 --version
Python 3.7.4
# pip3.7 --version
pip 19.2.3 from /usr/local/lib/python3.7/site-packages/pip (python 3.7)
```

**Thoughts:** Daunting but I like the idea of being held accountable. Not looking for perfection, but rather consistency and deliberate practice :)

**Link to work:**  

### Day 2: 20191002, Wed

**Today's Progress**: 

* Python 3 Scripting for System Administrators - Interacting with files
* exercies 1-3, key points to remember are setting variables up front, then iterate over the list/dict, modifying the var as you go, printing its value at the end. Use += to concatenate. Going forward, think about how you can use other functions to populate those dicts/lists. 

**Thoughts:**:  Wrote my own code before looking at the solution. I need to remember to keep it simple at first. For instance, I tried to do list.append(dict) but should have just defined the list of dicts without making the dicts variables. 


### Day 3: 20191003, Thu

**Today's Progress**: 

* Python 3 Scripting for System Administrators - pip, virtualenv, third party packages review
* Learning Python (linkedin) - vscode python extension config, fetching internet data, working with JSON

Finally get to work with real data, and also get a better understanding of main() funtion and what it means to a project with potentially multiple functions split over multiple files. 

**Thoughts:**:  I wonder if there is a better way to grab deal with deeply nested dictionary or list items instead of typing them all out. Also, is the json function in requests library same as the json library? Need to spend more time figuring out third party libs.

### Day 4: 20191004, Fri

**Today's Progress**: 
* Python: XML, JSON, and the Web (linkedin) - Requests and JSON
* Code Clinic: Python (linkedin) - POST with requests library

Found out GCP console has an API dashboard and seems there's no free tier anymore. 
Learned the difference between Request module and Requests package/library. Former is basic without POST capability, the latter you need to download but more robust. Wrote some code for grabbing tokens via API. 

**Thoughts:**:  need to tweak vscode a little more so that I can use 3rd party packages. 

### Day 5: 20191005, Sat

**Today's Progress**: 
Reorganizing existing code so that I have a main function that calls separate functions that include getting tokens, then POSTing some other data. Understanding where "return" is used in comparison to print functions. 

Learned about .get() vs using brackets in dictionaries. Also the new python3 print function has sep='\n' to printout items on separate lines. 

**Thoughts:**: Still lots to cover, but definitely making gains on fundamental concepts. 

### Day 6: 20191006, Sun

**Today's Progress**: 
Fixed my dictionary key check. 
Need to learn more about the while , if, continue concepts.  Especially in terms of continue and break, and what parts get looped, and what doesn't. 

**Thoughts:**:  parts of a script can get large quick...I can see why it's so hard to write simple yet understandable code...but when you start using code to simplify, that may not be the easiest to understand. 

### Day 7: 20191007, Mon

**Today's Progress**: 
Taking a side step to work on building out a CDN for a work project. 
Before that, I wanted to make all provisioning tools run in a container so working on a new multistage build dockerfile that apparently grabs all the necessary stuff from existing builds. Pretty interesting but need to play around with it. 

**Thoughts:**: Multi-tasking is inevitable. But it may prove helpful in keeping my interest going over time so I don't get burned out. 

### Day 8: 20191008, Tue

**Today's Progress**:  Did more work on terraform creating root module and child modules to spin up a network, subnetwork, firewall, f5 instance and nginx instance in that network. Created dockerfile that builds an alpine instance with terraform and ansible. Works great so far. 

**Thoughts:**:  IaC is also coding right? It also jives well with the https://12factor.net/ philosophy which I'm trying to absorb more of to put meaning to some of what I'm doing. For instance, is one container suppose to only have one process running on it or can we diverge?

### Day 9: 20191009, Wed

**Today's Progress**: Worked on my dockerfile more, merging in some code from SNOPS container so that it is able to run scripts that call git clone for a repo that I specify in an env variable in the .env file. Also has a mechanism to read a user-mounted json file that contains a repo location so that the user can specify his/her own repo without modifying the dockerfile or scripts. Cool idea so I wanted to try it out. This counts as python study because I had to understand how the script works. 

**Thoughts:**: Recent python study really came into play today while I looked at python code. Makes much more sense to know at least some of the basics. Even what I don't know I can figure out by context. Also figured out that bash scripting is similar enough to python so could understand it as well. 

### Day 10: 20191010, Thu

**Today's Progress**: Worked more with the CDN project. Completed the ansible playbooks/roles and tf modules. Also fixed the dockefile in multiple places. While not completely coding in Python, lots of the thought processes are similar to me. 

**Thoughts:**: Good to know the details of ansible and terraform. 

### Day 11: 20191011, Fri

**Today's Progress**: Didn't do a commit due to travel, but worked on understanding how terraform can output variables to a file using templates (.tpl) which can then be consumed by other tools like Ansible. Also spent time on reviewing basics of classes and for, while loops on linkedin learning.

**Thoughts:**: Can't let up just because of being on the road. Will keep moving forward but won't let a commit be overlooked again.

### Day 12: 20191012, Sat

**Today's Progress**:
Finished sections on shutil, zipfile, xml.dom.minidom and html parsing, and realized it could be used for "responsible" web scraping with robots.txt, then a whole can of worms explode

**Thoughts**: I should take time to google some practical use cases for some of the sections to connect the dots. 

### Day 13: 20191013, Sun

**Today's Progress**:
Finished some nginx training. Configuration shares a lot of similarities with javascript and other programming languages, but also key differences that can also be traps for those used to programming. 


### Day 14: 20191014, Mon

**Today's Progress**:
Linux Academy: More classes, composition, and inheritance. I realize this pattern of modularization appears in many different places hence me spending time here.  


### Day 15: 20191015, Tue

**Today's Progress**: 
Trying out Pomodoro method, and so far I like it. 
Learned more about argv vs argparse, which is actually what my side project scripts are using. 
Spent time adding gke creation to terraform and ansible. 

### Day 16: 20191016, Wed

**Today's Progress**: 
My licensing script works! Great feeling. I made the license key, ip address, username and password arguments that the user can pass in from the terminal. I can now use it as a stepping stone to more complex scripts. 
I will call it a night so I can catch up on sleep...

### Day 17: 20191017, Thu

**Today's Progress**: 
Cleaned up yesterday's script. Colleague told me that I should try to convert python to c to really learn some deep stuff. 
still haven't caught up on sleep but pushing through.

### Day 18: 20191018, Fri

**Today's Progress**: 
Learned more about err handling and try except block with finally. Went over my existing code to see where I could clean it up, add comments so I can remember why I did what. 
Spend a lot of time cleaning up also my terraform project. What a mess it was, with wrong module names, non-exiting input and output vars, but it did feel good to see successful "terraform validate" and "terraform plan". 

### Day 19: 20191019, Sat

**Today's Progress**: 
So while my tf validate succeeded, tf apply resulted in many errors, mostly due to not having the right output vars, not using self_link for the image name, some weird template_file error with curly brackets, etc. It was rough but I did feel good seeing the apply complete appear in that old school green on my black console background. 

I also managed to stick in some linux academy learning on list comprehensions and also executing shell commands in python. 
I can see how all of this has application in the real world. For now, going to bed. 

### Day 20: 20191020, Sun

**Today's Progress**:
Not much coding, more learning on linux academy. Ran through the random and json libraries. 
Even looking at the example code and listening to the instructor walk through the logic helps to understand more about design and syntax. Things like "with" for file open/close, and list comprehensions come up often so helps to remember it. 

Slowly but surely. 

### Day 21: 20191021, Mon

**Today's Progress**:
In linux academy, learned about OSError, glob/globbing syntax (to match multiple patterns of filenames), and shutil for doing operations on files. Spent most of my time today working on the CDN solution so not much coding. Caching is really a huge can of worms...but quite interesting to me to look at what people have been building over the years to optimize traffic. 

### Day 22: 20191022, Tue

**Today's Progress**:
Learned about re module in Linux academy, and was reminded that I need to practice more regex. Other than that I fixed my terraform so that it uses the new templatefile function introduced in 0.12. Now moving on to Ansible, and hitting the typical permissions errors that should be relatively easy to fix. 

### Day 23: 20191023, Wed

**Today's Progress**:
Learned a little about test driven development (TDD) and how it's part of extreme programming (XP). 
Starting to connect the dots a little with past devops events where David Bernstein talklkd about what it means to be Agile. 
Also used up cycles fixin my yaml files for Ansible to automate my infra more. lots to do!

### Day 24: 20191024, Thu

**Today's Progress**:
Made major strides in my IaC project. Kubeconfig file generation using terraform and yaml templates. 
This allows using the k8s module in ansible to then create a namespace and then a pod and service, granted the yaml manifest file is written correctly without syntax errors ;). 
While not much python, lots of similarities. 

### Day 25: 20191025, Fri

**Today's Progress**:
Looked at generating dump files. Nothing much else today as I was out and about almost all day getting some fresh air...and rain.

### Day 26: 20191026, Sat

**Today's Progress**:
Switched to a different course on linux academy that teaches python development. Same general content but good to go through for repetition and I also tend to pick up new things when doing something a second or third time. 
For instance, I start to think of the use cases where one would use tuples, dicts, ranges, and using tuples or lists to populate a dict. 
On the IaC side, I finally was able to get a successful playbook run with ansible. Ensured I used become_method: sudo. 

### Day 27: 20191027, Sun

**Today's Progress**:
Worked mainly looking at sed and regex to see how python can be used for the purpose of manipulating strings. Likely this can be done by using shutil and regex (re). 
Interesting topic. 
For my IaC project, I added in F5 instance to the terraform side, which required some output var fixes. Also plugged it into my ansible playbook, which required me adding paramiko and make to the list of apps to install in my alpine build, as well as dealing with some host_key_checking issues, which I hope to solve in the dockerfile. 

### Day 28: 20191028, Mon

**Today's Progress**:
Mostly doing work on terraform and ansible. 

### Day 29: 20191029, Tue

**Today's Progress**:
Studied about polymorphism and inheritance. I like the idea of not having to reinvent the wheel. Also need to ensure I practice this going forward. It can get confusing with all the moving parts...