Jenkins plugin for Acunetix 360

## Description

Allows users to start security scans via Acunetix 360 and see their
reports in Jenkins 

## Features

### Global Settings

Acunetix 360 plugin needs the admin user to define the API settings
only once.

![](ss/jenkins_global_settings.png)

### Global Settings Override

Global settings can be overridden in pipeline scripts by
giving ncApiToken and/or ncServerURL parameters.

#### Example Script

step([$class: 'NCScanBuilder', ncScanType: 'FullWithPrimaryProfile', ncWebsiteId: '19011b1b-4141-4331-8514-ab4102a4c135'])

![](ss/NE_jenkins_new_integration.png)

### Scan Settings

Once you define global API settings, the plugin retrieves available
scan settings such as scannable website list and scan profile names. You
can easily select relevant settings.

![](ss/jenkins_scan_settings.png)
  
### Scan Report

 Once your initiated scan is completed, you can easily see your
executive scan report on the build result window.

![](ss/jenkins_scan_report.png)

## Requirements

In order to use the Acunetix 360 scan plugin, following requirements
needs to be satisfied:

-   The user must have API token which has permission to start security
    scan.

-   The token belongs to the Acunetix 360 account must have at least one
    registered website. 

## User Guide

Acunetix 360 Jenkins Plugin documentation is always available at:

<https://www.acunetix.com/> (Will be updated)

Acunetix 360 SDLC documentation is always available at:

<https://www.acunetix.com/> (Will be updated)
