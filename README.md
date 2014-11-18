DataPow
=======

A web admin tool powered by Ruby on Rails and Twitter Bootstrap to manage various DataPower tasks from a centralized site. The calls to the DataPower devices are made via soap requests to the XML management interface. The SOAP constructors are modular and reusable, so when new features are needed, you spend less time developing and constructing soap messages.

There are various roles mapped and controlled within DataPow, for example Developers, Administrators, Operators, Enhanced Developers, etc. The different roles are mapped to certain functions and features within the tool to limit and control access.

Here is a snapshot of the 'hosts' page. Hostnames and serial numbers are blanked out, but the page shows pertinent information related to each device. This is useful to get the health status and general info / inventory of devices. The hosts displayed on the page are grouped in high-level buckets, so there are multiple groups in this page and below it. I only am showing the first bucket to keep it simple.

![ScreenShot](DataPow/master/images/hosts2.png)

Here are snapshots of the 'Resource Utlization' page. The memory and cpu resources are captured and written to a database via a cron job and displayed to the page. The intervals allow you to specify minute (up to 24 hours), 10 minute (up to 2 weeks), and hourly (up to 2 months). This is useful for capacity planning, load testing, and root cause analysis.
