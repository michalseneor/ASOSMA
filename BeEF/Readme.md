
# ![](https://github.com/rivkage/ASOSMA/blob/master/BeEF/beef.png) The BeEF Project 

 Team Members:  Sarah Gabriel,([SarahGabriel](https://github.com/SarahGabriel))
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

  The framework works with a client server architecture and different usage patterns level. The actors are mainly the user interface which is the control interface for using BeEF and the communication server. From the interface a user can see all online and offline browsers, run exploits against them and see the results while the communication server is the component that communicates via HTTP with the hooked browsers.  
  
  
 ![](https://github.com/rivkage/ASOSMA/blob/master/BeEF/Pattern1.png)  
 
 
  ![](https://github.com/rivkage/ASOSMA/blob/master/BeEF/highLevel.png)
  
#### Ressources
  
  BeEF is an actively developed open source project that allows the use of versioning systems such as Git ([repository](https://github.com/beefproject/beef)) and was nominated among toolswatch.org’s top 10 security tools. Each progress and improvement is shared through its [website](http://beefproject.com/), social networking ([twitter](https://twitter.com/beefproject), [Linkedin](https://www.linkedin.com/groups/3988552/profile)), an active [blog](http://blog.beefproject.com/) and a [youtube](https://www.youtube.com/user/TheBeefproject) channel. It was also the topic of many [reviews](https://github.com/beefproject/beef/wiki/References) and podcasts. Also, through the publication of the "Browser Hacker's Handbook", Wade has shared his specialist knowledge of security with students and professionals alike.  
  Also BeEF has a standard mailing list:  beef-subscribe@bindshell.net and a development mailing list: beef-dev-subscribe@bindshell.net
  
#### Development Process
  
  The development process is based on proactive communication and rotates around seven dates in the month. Each one of those dates represents a deadline for specific task concerning assignement of development goals, completion of issues, testing, verification and release of the result ([development cycle](https://github.com/rivkage/ASOSMA/blob/master/BeEF/DevelopmentCycle.md))
  
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
     
       
 
