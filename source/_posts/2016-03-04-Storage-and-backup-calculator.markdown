---
layout: post
title:  "Calculate TCO for storage and backup"
description: "Friendly folks over at AWS have released an online TCO calculator for storage use cases. Here is my take on it."
date:   2016-03-04 17:04:43
keywords: "Storage, Backup, TCO, AWS, AWS Solutions Architect, Cloud Automation, Cloud Architect, S3, Simple Storage Service"
comments: true
category: opinion
---
<p>What, do you think, is the simplest way to chop off a few percentage points of your IT budget? Does migrating to <a href="http://aws.amazon.com/">AWS cloud</a> storage come to mind? If not, think again! If you need help thinking, you may be in luck. The friendly folks over at AWS recently released a new <a href="http://www.backuparchive.awstcocalculator.com/">TCO calculator</a> for backup and archiving. It looks pretty cool; I took it for a drive earlier today. </p>
<p>
<a href="http://www.backuparchive.awstcocalculator.com/"><img src="/images/aws-tco-calculator.PNG" alt="Screenshot of AWS TCO calculator"/></a>
</p>
<p>It has three tabs, the <strong>basic</strong>, <strong>advanced</strong> and the <strong>direct</strong> tab. On the basic tab, you just enter the RAW storage that you currently have on-prem and a few characteristics of it, such as its y-o-y growth. Hit calculate, and AWS will show you a pretty picture of how AWS backup solutions compare with on-prem backup architectures. You can also compare the AWS solution with a colo architecture by choosing it in the drop down menu. On the Advanced tab, there are many more options to pick between warm backup and long term archival. If your organization has legal or regulatory requirements around backup, you can specify retention periods (in years or days or any term in between). On the advanced tab, you should also enter how often or how much of your data do you expect to restore and how many levels of redundancy do you want. Additionally, to truly compare on-prem costs with the cloud, the TCO calculator also allows you to enter your leverage of discounts and existing vendor relationships. This means that if you have an existing relationship with NetApp that allows you a 50% discount on volume purchases, this TCO calculator will shave that off its calculation of on prem costs. All in all, it seems well organized. Here is one of the calculations of my driving test on this calculator. I used numbers from a previous job where I was fairly conversant with data backup and archival.  
</p>
<p>
<a target="_blank" href="/images/aws-tco-calculator-test-drive.PNG"><img src="/images/aws-tco-calculator-test-drive.PNG" alt="Screenshot of AWS TCO calculator with my test drive numbers"/></a>
</p>
<p>
This is very interesting. At the very least, it shows two things. At first, it shows a clear cut, numbers based approach that you can compare to your own operations. Secondly, it offers a financial framework to think about cloud data backup and storage. Think about hot storage, cold storage, networking, personnel and support. Don't think vendors, appliances, hardware, disks, failures and any of those things that vex you today. Great job AWS! 
</p>
