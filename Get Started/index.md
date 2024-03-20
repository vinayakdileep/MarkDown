---
publishDate:
title: "Call API from Azure Function"
linkTitle: "Call from Azure Function"
author: vinayak
date: 2024-02-28
weight: 30
description: Invoke API from an Azure Function
hide_feedback: true
---



## Overview

Here, you will learn how to invoke the API from an Azure Function, utilizing the acquired token obtained using the SSO values from the payload.

For this tutorial, you need to ensure:

- You possess the credentials required for calling the API.


## Steps to configure

### Step 1: Configure Environment Variables in Azure Function App

configure something here

### Step 2: Populate SSO values and obtain the authorization token

Give some dummy details here.

#### Step 2.1: Retrieve SSO information

**Azure Function invoked from the event1:**

Here is an illustration of the payload structure and an explanation of how to extract SSO values from the payload when an Azure Function is invoked.

View the structure of the payload in the "Sample Payload" if the Azure Function is triggered.

some dummy details here.
<details>
<summary>Method to retrieve SSO information</summary>

```csharp
private static SSOInfo GetSSOValues(dynamic data)
{
    //retrieve the value from the global variable ApiConfidentialClientSecretKey in the app
    

    return ssoInfo;
}

public class SSOInfo
{
   //...................

}
```

</details>

**Azure Function invoked from the Event 2:**

Here is an illustration of the payload structure and an explanation of how to extract SSO values from the payload when an Azure Function is invoked from dummy event 2.

View the structure of the payload in the "Sample Payload" if the Azure Function is invoked by an dummy event.

<details>
<summary>Sample Response</summary>
{{< readfile file="json/employee.json" code="true" lang="json" >}}
</details>
