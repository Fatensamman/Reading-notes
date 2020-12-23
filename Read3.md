## Local Version Control

### Git Tutorial: A Comprehensive Guide:

- Version Control: used to understand Git 

- Version Control is a system which enables you, by saving changes, to revisit various versions of a file or collection of files. With version control, a file or project can be reversed in a previous version, changes can be monitored and improvements made and changes compared.

- Mistakes with files can be quickly corrected by the use of the VCS (Version Control System).
 

### Local Version Control:

- Local Version Control Systems were developed by programmers many years ago. A Local VCS contains one on your hard disk database which stores file changes.


### Centralized Version Control:

- The need for coordination on a single file or collection of files within the developer team led to the introduction of the Centralized Version Control System. This system contains a single server, which stores all modifications and variations of files that different clients can access. This simplified the coordination process (by removing the need to include all local databases), allowed programmers to know more about team members' activities with some files, and gave administrators much more power over the rights of revision.


### Distributed Version Control

- The key limitation of CVS is solved by a distributed version control system (DVCS): the server as a single fault point. When a CVS fails, collaborators cannot operate on a file, save changes and new versions with each other. Furthermore, all work, except for some portion of the local machine, is lost if the hard disk of a central database is corrupt— without any backups.

- A DVCS allows clients to build mirrored repositories to avoid this type form of catastrophic failure. These data backups can be put easily on the server to replace missing data.


### What is Git?

- Git is a DVCS which stores data in a snapshots file system. Git produces a snapshot of the file and stores a reference to the file any time you save the modified version of your project -named commit-. If the file has not modified, Git stores just the same version of the file.


### Local Operations:

- Git relies more on local operations because local resources are most likely to find the most important information.

- This enables the process to be simple, since the project history lies on the local drive, removing the need for the server to gather history information, and allowing you to continue working on a project even if you are not online or on a VPN.


  ### Benefits of Git

**Tracking Changes:**

- Git is monitored for each update applied to a file or a directory. And Git still recognizes file corruption or data loss as the gatekeeper.

**Loss of Data** 

- Git is set to reduce irreversible file damage, including accidental data loss, considerably. For your snapshot file, Git makes it incredibly difficult to lose.

**States**

- Git files can be committed, updated and staged