# Overview
The BMC AMI DevX Total Test extension can be used to execute either Unit or Functional test scenarios automatically. 

# BMC AMI DevX Total Test

This allows your GitHub Actions workflow to execute an automated test using Total Test. This action uses Total Test scenarios stored in your local Eclipse workspace. <br>
          
# Table of Contents

  * TTT-CLI-Local
    * [Table of Contents](https://github.com/marketplace/actions/bmc-ami-devx-total-test/#Table%20of%20Contents)
    * [Prerequisite](https://github.com/marketplace/actions/bmc-ami-devx-total-test/#Prerequisite)
    * [Usage](https://github.com/marketplace/actions/bmc-ami-devx-total-test/#Usage)
    * [Inputs](https://github.com/marketplace/actions/bmc-ami-devx-total-test/#Inputs)
    * [Outputs](https://github.com/marketplace/actions/bmc-ami-devx-total-test/#Outputs)
    * [Troubleshooting](https://github.com/marketplace/bmc-ami-devx-total-test/#Troubleshooting)
    * [License summary](https://github.com/marketplace/actions/bmc-ami-devx-total-test/#License%20summary)
    * [Product Assistance](https://github.com/marketplace/actions/bmc-ami-devx-total-test/#Product%20Assistance)

# Prerequisite

 * You can host your own runners and customize the environment used to run jobs in your GitHub Actions workflows, Click [here](https://docs.github.com/en/actions/hosting-your-own-runners/about-self-hosted-runners).
 * User need to setup BMC AMI DevX workbench CLI into local system.
 * User has to setup the MF password in github repository with the following steps
   * "Github Repository" -> Settings-> Secrets-> Actions-> New repository secret

# Usage

* Triggers the workflow to execute the provided test scenario on any pipeline where the BMC AMI DevX Total Test Auto Run is added. 
* Steps to use the extension
  * Install the BMC AMI DevX workbench CLI into local system, Click [here](https://download.api.compuware.com/web/private/66jvM2Rf5dcHtVjXdYhudGtRn9CtHzYq/test-management/results.html).
  * CLI Execution path - Go to the local drive of a system and check the .bat file location i.e "C:\\BMC AMI DevX\\topazworkbenchcli.20.12.03.134\\".
  * HCI Connection - Provide the HCI connection i.e CW01.bmc.com
  * Port - Provide the HCI connection port number i.e 16196
  * Test Location Path - Test location path is your local path where you test cases being executed i.e    "C:\\Users\\your_username\\BMC\\Workbench\\workspace\\CLI_CWKTCOBX\\Tests\\Scenarios"
  * CLI path - Provide the CLI path where a workspace available i.e. "C:\\Users\\your_username\\git\\TTT\\work\\workspace\\Security_Vulnerability\\TopazCliWkspc"
  * Repository server - Provide the repository server location i.e. "http://vw-dtw-xat-01.adprod.bmc.com:48231/totaltestapi/"
  * HCI user id - Provide you user id which can connect to MF
  * Password - Configure you MF password in "Github Repository" -> Settings-> Secrets-> Actions-> New repository secret
     
 
# Inputs


| Input name | Required | Description |
| --- | --- | --- |
| CLI Execution path | Required  | CLI execution path is the location where it is installed locally, provide path till .bat folder  |
| HCI Connection | Required  | HCI connection required to connect the MF system |
| HCI Connection Port  | Required  | HCI connection port is required to connect the system |
| Test Location Path | Required  | Test location path is your local path where you test cases being executed |
| workspace  | Required  | workspace is required for local setup |
| repository_server  | Required  | Repository server is required to connect and get the data from the server |
| User ID  | Required  | Provide your Mainframe User ID |
| Password  | Required  | "Github Repository" -> Settings-> Secrets-> Actions-> New repository secret |


# Outputs

Output will saved in Output folder created under Test Location Path in your local system.

# Troubleshooting

To enable debug logging in your GitHub actions workflow, see the guide [here](https://docs.github.com/en/actions/monitoring-and-troubleshooting-workflows/enabling-debug-logging).

# License summary

This code is made available under the BMC license, Click [here](https://github.com/bmc-compuware/TTT-CLI-Local/blob/main/LICENSE.txt).

# Product Assistance

BMC provides assistance for customers with its documentation, the BMC Support Center web site, and telephone customer support.

### BMC Support Center

You can access online information for BMC products via our Support Center site at [https://support.bmc.com](https://support.bmc.com/). Support Center provides access to critical information about your BMC products. You can review frequently asked questions, read or download documentation, access product fixes, or e-mail your questions or comments. The first time you access Support Center, you must register and obtain a password. Registration is free.

### Contacting Customer Support

At BMC, we strive to make our products and documentation the best in the industry. Feedback from our customers helps us maintain our quality standards. If you need support services, please obtain the following information before calling BMC\'s 24-hour telephone support:

- The Azure pipeline job output that contains any error messages or pertinent information.

- The name, release number, and build number of your product. This information is displayed in the installed extensions page. Apply filter: BMC in order to display all of the installed BMC extension.

- Environment information, such as the operating system and release on which the Topaz CLI is installed.

You can contact BMC in one of the following ways:


#### Web

You can report issues via BMC Support Center: [https://support.bmc.com](https://support.bmc.com/).

Note: Please report all high-priority issues by phone.

### Corporate Web Site

To access BMC site on the Web, go to [https://www.bmc.com/](https://www.bmc.com/). The BMC site provides a variety of product and support information.


   
