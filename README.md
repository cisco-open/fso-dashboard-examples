# FSO Dashboards Demo Repository

This repository contains the demo dashboards that are packages in FSO. You can learn more about the FSO Platform [here](https://developer.cisco.com/docs/fso/#!platform-overview)

## Dashboards Included

### APM
![APM Dashboard Screenshot](objects/dashboards/apm/apm.png?raw=true "APM Dashboard Screenshot")

## How to use it

Install & use fsoc: https://github.com/cisco-open/fsoc
Once installed follow these commands

fsoc solution package --solution-package=dashboardsDemo
fsoc solution validate --solution-bundle=dashboardsDemo.zip

fsoc solution push --solution-bundle=dashboardsDemo.zip
fsoc solution subscribe --name=dashboardsDemo
fsoc solution status --name=dashboardsDemo

fsoc objstore get --type=dashboards:dashboard --layer-type=TENANT

More details on how to currently upload a solution and troubleshooting can be found [here](https://developer.cisco.com/docs/fso/#!troubleshoot-solutions)

If you have to change something in this repository, remember to bump the version in the [manifest.json](manifest.json)
