## Cartridge for bpmPaaS with HR Employee Rewards Demo

This cartridge provides the **_Red Hat JBoss BPM Suite_** for easy deployment to OpenShift based bpmPaaS with pre-loaded Employee
Rewards Demo.

Setup Now
---------
1. Login to OpenShift Origin and go to the [OpenShift create application page](https://openshift.redhat.com/app/console/application_types).

2. In `CODE ANYTHING` field at bottom left of the page paste the following cartridge URI:

     _https://raw.githubusercontent.com/eschabell/cartridge-bpmPaaS-rewards-demo/master/metadata/manifest.yml_

3. Click on `NEXT` button and drink a warm beverage while you wait for finished cartridge installation.

Once installed you can use the JBoss BPM Suite logins: 

   * u:erics  p: bpmsuite  (admin)
   
   * u: alan  p: bpmsuite  (analyst)
   
   * u: daniel  p: bpmsuite  (developer)
   
   * u: ursla  p: bpmsuite  (user)

   * u: mary  p: bpmsuite  (manager)


Important Note
--------------
You need the ability to setup MEDIUM gears, which is freely available if you [upgrade your account to Bronze here] (https://www.openshift.com/products/pricing). 


Deployment
----------

Or if you want to use the [rhc command line](https://www.openshift.com/developers/rhc-client-tools-install) type:

    rhc app create -g medium <APP NAME> https://raw.githubusercontent.com/eschabell/cartridge-bpmPaaS-rewards-demo/master/metadata/manifest.yml

For more information on the [HR Employee Rewards Demo see here] (https://github.com/eschabell/bpms-rewards-demo).

Supporting Articles
-------------------

[Real life bpmPaaS with JBoss BPM Suite HR employee rewards demo] (http://www.schabell.org/2014/06/real-life-bpmpaas-with-jboss-bpmsuite-rewards-demo.html)


Released versions
-----------------

See the tagged releases for the following versions of the product:

- v1.1 - bpmPaaS on OpenShift cartridge, JBoss BPM Suite 6.0.2 and Rewards demo installed.

- v1.0 - bpmPaaS on OpenShift cartridge, JBoss BPM Suite 6.0.1 and Rewards demo installed.

![Rewards Process](https://github.com/eschabell/bpms-rewards-demo/blob/master/docs/demo-images/rewards-process.png?raw=true)

