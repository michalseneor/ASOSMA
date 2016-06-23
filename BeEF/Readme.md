
# ![](https://github.com/rivkage/ASOSMA/blob/master/BeEF/beef.png) The BeEF Project 

 Authors:  Sarah Gabriel,([SarahGabriel](https://github.com/SarahGabriel))
                Ran Itzhaki ([ranitz](https://github.com/ranitz)), 
                Itsik Rabinovitch ([itzikrb100](https://github.com/itsikrb100)), 
                Rivka Gehler ([rivkage](https://github.com/rivkage)),
                Mihal Seneor ([michalseneor](https://github.com/michalseneor))


## Introduction
  
   BeEF is short for **The Browser Exploitation Framework**, a powerful professional security tool. It was founded by Wade Alcorn the NGS Security's general manager for Asia Pacific, leaded by Christian Fricho, leader of the Perth Open Web Application Security Project and Michelle Orru a vulnerability researcher and social engineer.
  
#### What is BeEF ?

  Unlike other security frameworks, BeEF focuses on leveraging browser vulnerabilities to assess the security posture of a target. 
  This project is developed solely for lawful research and penetration testing.   
  BeEF looks past the hardened network perimeter and client system, and examines exploitability within the context of the one open door: the web browser. BeEF will hook one or more web browsers and use them as beachheads for launching directed command modules and further attacks against the system from within the browser context. Each browser is likely to be within a different security context, and each context may provide a set of unique attack vectors.
  The framework contains numerous command modules that employ BeEF's simple and powerful API. This API is at the heart of the framework's effectiveness and efficiency. It abstracts complexity and facilitates quick development of custom modules.
  The penetration tester can then select specific modules (in real-time) to target each browser, and therefore each context.  
  
#### Architecture 

  The framework works with a client server architecture and different usage patterns level. The actors are mainly the user interface which is the control interface for using BeEF and the communication server. From the interface a user can see all online and offline browsers, run exploits against them and see the results while the communication server is the component that communicates via HTTP with the hooked browsers. The following high level diagrams are from the BeEF [wiki](https://github.com/beefproject/beef/wiki/Architecture)  
  
  
 ![](https://github.com/rivkage/ASOSMA/blob/master/BeEF/Pattern1.png)  
 
 
  ![](https://github.com/rivkage/ASOSMA/blob/master/BeEF/highLevel.png)
  
#### Ressources
  
  BeEF is an actively developed open source project that allows the use of versioning systems such as Git ([repository](https://github.com/beefproject/beef)) and was nominated among toolswatch.org’s top 10 security tools. Each progress and improvement is shared through its [website](http://beefproject.com/), social networking ([twitter](https://twitter.com/beefproject), [Linkedin](https://www.linkedin.com/groups/3988552/profile)), an active [blog](http://blog.beefproject.com/) and a [youtube](https://www.youtube.com/user/TheBeefproject) channel. It was also the topic of many [reviews](https://github.com/beefproject/beef/wiki/References) and podcasts. Also, through the publication of the "Browser Hacker's Handbook", Wade has shared his specialist knowledge of security with students and professionals alike.  
  Also BeEF has a standard mailing list:  beef-subscribe@bindshell.net and a development mailing list: beef-dev-subscribe@bindshell.net
  
#### Development Process
  
  The development process is based on proactive communication and rotates around seven dates in the month. Each one of those dates represents a deadline for specific task concerning assignement of development goals, completion of issues, testing, verification and release of the result ([development cycle](https://github.com/beefproject/beef/wiki/Development-Organization)
  
#### Guidelines

 To submit an issue, contributors should do it according to guidelines and an [issue template](https://github.com/beefproject/beef/blob/master/.github/ISSUE_TEMPLATE.md). Submitter will have to fill all the fields so that the issue environment could be reproduce and then fixed. It allows a better platform maintenance.  
 
#### Graphs and Statistics

**Contributions to master:**  (https://github.com/beefproject/beef/graphs/contributors)   
![](https://github.com/rivkage/ASOSMA/blob/master/BeEF/ContributionToMaster.PNG)  

**Weekly Commits:** (https://github.com/beefproject/beef/graphs/commit-activity)
![](https://github.com/rivkage/ASOSMA/blob/master/BeEF/WeeklyCommits.PNG) 

 **Bug/Features list in the [issues](https://github.com/beefproject/beef/issues) section on github:**  (bugs/features are tagged according to their importance and type) 
  
  ![](https://github.com/rivkage/ASOSMA/blob/master/BeEF/bugs_featuresList.png)

#### Why did we choose BeEF ?

   BeEF stands for a platform in constant evolution and a tool that meets people growing needs of a secure environment in a web focused world. It has been restructurated from a Php application to a Ruby base framework, allowing  many new features to be added and its community to grow, handling now pull requests daily.  
   This makes BeEF a great choice for a Software Architecture analysis.  
   In this project, insights regarding BeEF's Software Architecture are given. This makes it easier for new people to join the open source scene to contribute to the BeEF project. Additionally this will also give the BeEF team an outsider's view of their Software Architecture.  
     
       
 
 
####**The Beef project documentation** 

We will discuss two perspectives of the given documentation:
 
1. The user's perspective – a user is someone who just want to use Beef.
The documentation for the BeeF newbie user is relatively comprehensive and including information about BeeF's project goals purposes and means.
The documentation includes installation instructions for different operating systems, command line usage, detailed configuration including screenshots and even small video clips that shows how to configure BeeF and run it. There is a very detailed section on BeeF's capabilities on different browsers.

2. The developer's perspective – a developer is someone who wants to contribute to the BeeF project by adding extensions or keep developing the code.  
The given documentation is not describing the source code and is not containing any detailed diagrams that can help the developers get familiar with the system faster, a developer that wants to know the code better in order to integrate with it will have to go over the entire code by himself and to assemble the whole picture in his head.
However the code is containing comments which can make the code learning process much faster. The documentation is containing information how to create new modules of our own, BeeF is built in a modular way so it is supposed to be easy creating new modules and adding them to BeeF. 
In generally we think that in order to create a new module the supplied documentation is rather sufficient but in order to get familiar with the rest of the code a lot of learning hours and code analysis will be needed.



####**Source Code Structure**
The code consists of ruby and JavaScript files.
The application itself is written in ruby and the code that is supposed to be injected in to the "victim's" browsers in order to check its vulnerability is written in JavaScript.
The code is built in a modular way so creating new modules and adding them to BeeF should be pretty easy, but as mention in the documentation section the core code of the project is complicated and requires a comprehensive code analysis.
Ruby code main classes:


![](https://github.com/itzikrb100/ASOSMA/blob/master/BeEF/pic1.png)


####**The Stakeholders**
The BeeF project comprises a large community of dozens of software engineers, developers and testers. They work on a voluntary base, as most of them have another job and no income is generated since BeeF is freeware, it is easy to assume that the developers come from the security information world or have a great affection to this field.
As it can be seen from the following figures the 2 leading contributors are contributing to other projects that are also dealing with the information security field. 


![](https://github.com/itzikrb100/ASOSMA/blob/master/BeEF/pic2-stakeholders.png)


We can classify the prominent stockholders into 3 groups:

**Core BeeF organization (Management)**

An information about this members is not supplied in their Github page nor in their website, while digging a little further in order to identify the core members led to the conclusion that a limited group of developers have the right to approve or deny the potential contributions and bug reports (the 2 guys mentioned above are surely a part of this group).

**Developers**

There is a certain group of developers that is continuously contributing to improve BeeF project. They reply, issue and close tickets when a bug is fixed. In that way they work closely with the users. From surfing in the BeeF's blog we saw that there are researches in the field of information security and cryptography that are participating in the BeeF project by developing experimental features. 
Suggesting new module to Beef Process:


![](https://github.com/itzikrb100/ASOSMA/blob/master/BeEF/pic3-Developers.png)

**Users**

Since the BeeF project is dependent on their users to use the system to assess the actual security posture of a target environment by using client-side attack vectors they embrace them to contribute to the continuous improvement of the web browsers penetration system by reporting bugs and proposing new modules. Also the web browsers companies themselves can benefit from using the framework in order to identify vulnerabilities in their browsers and close  them.





####UML Modeling Diagrams

**describe the main login attack:**

   **usecase diagram -**

 ![](https://github.com/itzikrb100/ASOSMA/blob/master/BeEF/use%20login%20tracker.png)


 **sequence diagram -**
 
 ![](https://github.com/itzikrb100/ASOSMA/blob/master/BeEF/sequence%20diagram%20login.png)


**description RESTful API sequence diagram :** In order to use the API, a token parameter must be always added to requests
 (Alternatively,if you want to write automated scripts that uses the RESTful API, you can issue a POST request to /api/admin/login using the BeEF credentials).After this The hooks handler gives information about the hooked browsers, both online and offline.
 

####**Challenges**


**We think that the BeeF project has 2 major challenges:**

1. staying relevant: the web browsers are always evolving, new versions are always released what makes it harder to hook them and find new exploitations.
In addition to this, new features and plugins are also being developed and released every day in growing rate for all platforms and operating systems: Windows, Linux, Andoird, IOS etc.., the BeeF project should create new modules that are able to exploit vulnerabilities in these new  features and plugins for all the mentioned platforms.
2. Hooking as much web browsers as possible for all relevant platforms and supplying the same functionalities to penetrate for all of the web browsers.


**Latest open major bugs**

1.  Geolocation not working on any chrome browser (Android, Windows, Linux, IOS). This issue was opened on 27/5/2016 by Nhoty and the developer Brendan Coles labeled this issue as a defect & module one day later (on 28/5/2016) that shows that issues are addressed quickly  although a fix for this issue haven't been released yet (1/6/2016). The issue means that the released module for geolocation is having a serious bug in chrome browser. [(https://github.com/beefproject/beef/issues/1269)](https://github.com/beefproject/beef/issues/1269)
All the other major bugs are from 2 years ago or more so we guess it was fixed in newer versions.

All the other major bugs are from 2 years ago or more so we guess it was fixed in newer versions.

**Missing important features**

1. IPV6 support, the current state of IPV6 support is not known.
2. API call to manually set OS and browser version of hooked browsers. [(https://github.com/beefproject/beef/issues/1164).](https://github.com/beefproject/beef/issues/1164)


3. Implement VNC style functionality in BeeF. This will allow real time monitoring of the hooked-browser’s view. That is, when the hooked browser follows a (onsite) link or enters content into input boxes it is viewed/monitored/recorded in the framework. The framework will have a proxy running on the loopback. When a browser connects to this proxy, the user can watch a playback or watch real-time with the user’s session.
