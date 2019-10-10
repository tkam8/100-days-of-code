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

### Day 9: 20191008, Wed

**Today's Progress**: Worked on my dockerfile more, merging in some code from SNOPS container so that it is able to run scripts that call git clone for a repo that I specify in an env variable in the .env file. Also has a mechanism to read a user-mounted json file that contains a repo location so that the user can specify his/her own repo without modifying the dockerfile or scripts. Cool idea so I wanted to try it out. This counts as python study because I had to understand how the script works. 

**Thoughts:**: Recent python study really came into play today while I looked at python code. Makes much more sense to know at least some of the basics. Even what I don't know I can figure out by context. Also figured out that bash scripting is similar enough to python so could understand it as well. 

### Day 10: 20191009, Thu

**Today's Progress**: Worked more with the CDN project. Completed the ansible playbooks/roles and tf modules. Also fixed the dockefile in multiple places. While not completely coding in Python, lots of the thought processes are similar to me. 

**Thoughts:**: Good to know the details of ansible and terraform. 