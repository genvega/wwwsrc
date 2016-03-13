---
layout: post
title:  "Tvarit is ready for takeoff!!"
description: "Tvarit (www.tvarit.io) is a devops automation tool for AWS. After months of painstaking development, it is now ready for a test flight."
date:   2016-03-12 17:04:43
keywords: "DevOps, DevOps Automation, Tomcat, AWS, AWS Solutions Architect, Cloud, Cloud Architect"
comments: true
category: announcements
---
<p><img src="/images/its_automatic-reduced.jpg" alt="AWS automated development operations"/></p>
<p>After weeks of burning the midnight candle, I have just released the <a href="https://github.com/sdole/tvarit-maven/releases/tag/v0.1.1-alpha">first working alpha</a> of <a style="font-weight:bold" href="http://www.tvarit.io">Tvarit</a> - a Dev Ops Automation tool for Amazon Web Services! It is in <a href="http://search.maven.org/#artifactdetails%7Cio.tvarit%7Ctvarit-maven-plugin%7C0.1.1%7Cmaven-plugin">maven central</a>; give it a spin! I want to hear your <a href="https://github.com/sdole/tvarit-maven/issues/new">feedback<a/>. Does it work for you? What <a href="https://github.com/sdole/tvarit-maven/blob/master/README.md">documentation</a> should I add to make it clearer? 
</p>
<p>
<h2>Features</h2>
<p>
In a nutshell, Tvarit enables a development team to completely automate deployment of a JEE WAR file to AWS. 
</p>
<p><ol>
    <li>1. Tomcat 8 application server with Java 8</li>
    <li>2. High availability via cross zone load balancing</li>
    <li>3. Completely automated infrastructure setup and deployment</li>
    <li>4. Scale horizontally using AWS's native autoscaling</li>
    <li>5. Customize using cloudformation templates (or use the default setup)</li>
</ol>
</p><p>
<h2>Roadmap</h2></p>
<p>This is already an exciting product. It can already shave of hours and hours of manual labor for a typical project running on the JEE platform! Here are some of the major enhancements I plan to make in the near future.
</p>
<p><ol>
    <li>1. Scale down previously running application versions</li>
    <li>2. Completely customizable application server environments</li>
    <li>3. Deploy with an RDS datasource with secured credentials<li>
    <li>4. Automatic independent environments for test and production</li>
    <li>5. Multi-app deployment and inter app-version contracts (à la micro-services)</li>
    </ol>
</p>
<p><h2>How can you help?</h2></p>
<p>There are many ways you can get involved. Have a feature idea on your mind? <a href="https://github.com/sdole/tvarit-maven/issues/new">Suggest it</a>, or submit me a pull request. Have questions? Ask me here (in the comments) or on <a href="https://github.com/sdole/tvarit-maven/issues/new">GitHub</a>. Not sure how you can help or have other questions? <a href="mailto:sdole@genvega.com?subject=I have a question about Tvarit">Email me</a> or <a href="https://twitter.com/sdoledotcom/">tweet me</a>, lets discuss!
</p>
<p><h2>How can I help?</h2></p>
<p>I am available for supporting Tvarit and for assessing your Dev Ops automation requirements. I am also available to discuss general AWS topics at your office, with your developers. If you have not already, please check some of my other articles here or come to one of my meetup sessions. AWS is a great product that can truly bring down the costs of your IT infrastructure while improving availability and scalability of it. Ask me to find out how you can do it!
</p>