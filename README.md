# Depricated: 

-----

This project was based on OpenShift v2, a new version is available 
for [OpenShift Container Platform](https://github.com/redhatdemocentral/rhcs-rewards-demo).

-----


Cartridge for bpmPaaS with HR Employee Rewards Demo
===================================================
This cartridge provides the **_Red Hat JBoss BPM Suite_** for easy deployment to OpenShift based bpmPaaS with pre-loaded Employee
Rewards Demo.


Install with one click in xPaaS (bpmPaaS)
-----------------------------------------
After clicking button, ensure `Gear` size is set to `medium`:

[![Click to install OpenShift](http://launch-shifter.rhcloud.com/launch/light/Install bpmPaaS.svg)](https://openshift.redhat.com/app/console/application_type/custom?&cartridges[]=https://raw.githubusercontent.com/jbossdemocentral/cartridge-bpmPaaS-rewards-demo/master/metadata/manifest.yml&name=rewards&gear_profile=medium&initial_git_url=)

Once installed you can use the JBoss BPM Suite login: 

   * u:erics   p: bpmsuite  (admin)

   * u: alan   p: bpmsuite  (analyst)

   * u: daniel p: bpmsuite (developer)

   * u: ursla  p: bpmsuite (user)

   * u: mary   p: bpmsuite (manager)

After claiming the user task as a manager (to approve or deny the award), if task completion takes longer
than 1 minutes it will te reassigned back into the group so other managers can claim it. The short time frame
of 1 minutes is for demo purposes, should talk about days to complete instead as if a manager that claimed a
task got sick and failed to complete the claimed task.

Note email notifications on user tasks will not work due to lack of port access. If you claim the task before 2 minutes expires and
let it sit for longer than 1 minute without completing it will automatically reassign the task to the group.

Important Note
--------------
You need the ability to setup MEDIUM gears, which is freely available if you [upgrade your account to Bronze
here](https://www.openshift.com/products/pricing). 


Manual setup on OpenShift
-------------------------
Or if you want to use the [rhc command line](https://www.openshift.com/developers/rhc-client-tools-install) type:

    rhc app create -g medium <APP NAME> https://raw.githubusercontent.com/jbossdemocentral/cartridge-bpmPaaS-rewards-demo/master/metadata/manifest.yml

For more information on the [HR Employee Rewards Demo see here] (https://github.com/jbossdemocentral/bpms-rewards-demo).


Supporting Articles
-------------------
[Launching Into the Clouds With 2 New OpenShift Primer bpmPaaS Quickstarts](http://www.schabell.org/2014/10/launching-into-clouds-with-2-new-openshift-primer-bpmpaas-quickstarts.html)

[Real life bpmPaaS with JBoss BPM Suite HR employee rewards demo] (http://www.schabell.org/2014/06/real-life-bpmpaas-with-jboss-bpmsuite-rewards-demo.html)


Released versions
-----------------
See the tagged releases for the following versions of the product:

- v1.3 - bpmsPaaS on OpenShift cartridge, JBoss BPM Suite 6.0.2 and Rewards demo with automated task reassignment.

- v1.2 - moved to JBoss Demo Central, added one click install button.

- v1.1 - bpmPaaS on OpenShift cartridge, JBoss BPM Suite 6.0.2 and Rewards demo installed.

- v1.0 - bpmPaaS on OpenShift cartridge, JBoss BPM Suite 6.0.1 and Rewards demo installed.


![Rewards Process](https://github.com/jbossdemocentral/bpms-rewards-demo/blob/master/docs/demo-images/rewards-process.png?raw=true)

