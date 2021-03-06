---
title: API
layout: rancher-api-v2-beta-default-v1.6
version: v1.6
lang: en
apiVersion: v2-beta
#redirect_from:
#  - /rancher/v1.6/zh/api/v2-beta/api-resources/genericObject/
---

## genericObject



### Resource Fields

#### Writeable Fields

Field | Type | Create | Update | Default | Notes
---|---|---|---|---|---
description | string | Optional | Yes | - | 
key | string | Optional | - | - | 
kind | string | Optional | - | - | 
name | string | Optional | - | - | 
resourceData | map[json] | Optional | - | - | 


#### Read Only Fields

Field | Type   | Notes
---|---|---
accountId | [account]({{site.baseurl}}/rancher/{{page.version}}/{{page.lang}}/api/{{page.apiVersion}}/api-resources/account/)  | The unique identifier for the associated account
created | date  | The date of when the genericObject was created.
data | map[json]  | 
id | int  | The unique identifier for the genericObject
removeTime | date  | The date and time of when the genericObject was removed
removed | date  | The date of when the genericObject was removed
state | enum  | The current state of the genericObject. The options are `activating`, `active`, `removed`, `removing`, `requested`.
transitioning | enum  | Whether or not the genericObject is in a transitioning state
transitioningMessage | string  | The message to show while in a transitioning state
transitioningProgress | int  | The percentage remaining in the transitioning process of the genericObject
uuid | string  | The universally unique identifier for the genericObject. This will always be unique across Rancher installations.


<br>
