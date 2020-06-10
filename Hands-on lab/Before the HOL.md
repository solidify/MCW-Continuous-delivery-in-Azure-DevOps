![Microsoft Cloud Workshops](https://github.com/Microsoft/MCW-Template-Cloud-Workshop/raw/master/Media/ms-cloud-workshop.png "Microsoft Cloud Workshops")

<div class="MCWHeader1">
Continuous delivery in Azure DevOps
</div>

<div class="MCWHeader2">
Before the hands-on lab setup guide
</div>

<div class="MCWHeader3">
December 2019
</div>

Information in this document, including URL and other Internet Web site references, is subject to change without notice. Unless otherwise noted, the example companies, organizations, products, domain names, e-mail addresses, logos, people, places, and events depicted herein are fictitious, and no association with any real company, organization, product, domain name, e-mail address, logo, person, place or event is intended or should be inferred. Complying with all applicable copyright laws is the responsibility of the user. Without limiting the rights under copyright, no part of this document may be reproduced, stored in or introduced into a retrieval system, or transmitted in any form or by any means (electronic, mechanical, photocopying, recording, or otherwise), or for any purpose, without the express written permission of Microsoft Corporation.

Microsoft may have patents, patent applications, trademarks, copyrights, or other intellectual property rights covering subject matter in this document. Except as expressly provided in any written license agreement from Microsoft, the furnishing of this document does not give you any license to these patents, trademarks, copyrights, or other intellectual property.

The names of manufacturers, products, or URLs are provided for informational purposes only and Microsoft makes no representations and warranties, either expressed, implied, or statutory, regarding these manufacturers or the use of the products with any Microsoft technologies. The inclusion of a manufacturer or product does not imply endorsement of Microsoft of the manufacturer or product. Links may be provided to third party sites. Such sites are not under the control of Microsoft and Microsoft is not responsible for the contents of any linked site or any link contained in a linked site, or any changes or updates to such sites. Microsoft is not responsible for webcasting or any other form of transmission received from any linked site. Microsoft is providing these links to you only as a convenience, and the inclusion of any link does not imply endorsement of Microsoft of the site or the products contained therein.

© 2019 Microsoft Corporation. All rights reserved.

Microsoft and the trademarks listed at <https://www.microsoft.com/en-us/legal/intellectualproperty/Trademarks/Usage/General.aspx> are trademarks of the Microsoft group of companies. All other trademarks are property of their respective owners.

**Contents**

<!-- TOC -->

- [Continuous delivery in Azure DevOps before the hands-on lab setup guide](#continuous-delivery-in-azure-devops-before-the-hands-on-lab-setup-guide)
  - [Requirements](#requirements)
  - [Before the hands-on lab](#before-the-hands-on-lab)
    - [Prerequisites](#prerequisites)
    - [Task 1: Use Azure Shell as your development environment](#task-1-use-azure-shell-as-your-development-environment)
    - [Task 2: Download the exercise files](#task-2-download-the-exercise-files)

<!-- /TOC -->

# Continuous delivery in Azure DevOps before the hands-on lab setup guide

## Requirements

1.  Microsoft Azure subscription

## Before the hands-on lab

Duration: 10 minutes

In this lab, you will configure a developer environment and download the required files for this course if you do not already have one that meets the requirements.

### Prerequisites

-   Microsoft Azure subscription <http://azure.microsoft.com/en-us/pricing/free-trial/>

### Task 1: Use Azure Shell as your development environment

>**Note**: This workshop *can* be completed using only the Azure Cloud Shell.   However, if you are a developer you should take the opportunity to use your local setup to perform the exercises. 

We have [a guide for local setup of the Azure CLI you can use ](http://hermit.no/how-to-setup-azure-cli-for-use-with-bash-shell-in-windows/).  

If you don't have Git installed locally, it can be [downloaded and installed from here](https://git-scm.com/download/win)

1.  In a web browser, navigate to https://shell.azure.com. Alternatively, from the Azure web portal, launch the **Azure Cloud Shell**. It has common Azure tools preinstalled and configured to use with your account.

    ![This is a screenshot of a icon used to launch the Azure Cloud Shell from the Azure Portal.](images/Setup/image3.png "Azure Cloud Shell launch icon")

2.  From inside the Azure Cloud Shell (or Azure CLI locally) type these commands to configure Git:

    ```bash
    git config --global user.name "<your name>"
    ```

    ```bash
    git config --global user.email <your email>
    ```

3. If you run locally, you should login to Azure using the Azure CLI

    ```
    az login
    ```

4. Locally you can use a Visual Studio developer command shell, or you can use the Git Bash shell.  

    Using Windows search, you can find either of these, searching for either 'developer' or 'bash'.

    Whenever the text below, or in the Hands On Lab refers to Azure Cloud Shell, you should use the Bash shell with Azure CLI.  (For most of the commands, you can use either (Dev Cmd or Bash) but when executing the script to upload the ARM template, you must use Bash.)  

    Note that if you didn't set up the alias shown in point 3 in the [guide](http://hermit.no/how-to-setup-azure-cli-for-use-with-bash-shell-in-windows/), then you must use the full name of the CLI like_

    ```
    az.cmd login
    ```
>**Note**: Using the Azure Cloud Shell, you
 can load the integrated code editor (Cloud Shell Editor) at any time with the following command:
```bash
code .
```

You should follow all steps provided *before* starting the Hands-on Lab.
