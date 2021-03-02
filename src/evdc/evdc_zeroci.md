# How to Deploy a ZeroCI server on eVDC

[ZeroCI](https://github.com/threefoldtech/zeroCI) is ThreeFold's own continuous integration tool for developers looking to build on top of the decentralized ThreeFold Grid.

It is useful for all languages, though it has some more specific features for Python projects that generates test summary into xml file. It is integrated with version control systems and Telegram.

# Get Started

You can now deploy your own ZeroCI server via the ThreeFold Marketplace's dashboard on your eVDC admin panel in a few clicks.

First step, find the **ZeroCI Widget** on the marketplace and click on **'Deploy'** button. You will now will be directed to the chatflow of the deployment process.

![](img/evdc_marketplace_zeroci_widget.png)

Create a name for your solution. This name will be used to identify your deployment on your `Deployed Solutions` list.

![](img/evdc_zeroci_01_name.png)

Select the domain type. For deployment with random subdomain, select `Choose subdomain for me on a gateway`. For deployment with a particular available subdomain, select 'Choose a custom subdomain on a gateway. To deploy a ZeroCI server using your own domain, select `choose a custom domain`.

![](img/evdc_zeroci_02_domain.png)

Select the VDC capacity plan for your ZeroCI server workload usage. This plan depends on the amount of workload you intend to store on the 

![](img/evdc_zeroci_03_flavour.png)

Congratulations! you just successfully deployed a ZeroCI server on the ThreeFold_Grid ! You can now click on the given link to access it.

![](img/evdc_zeroci_04_success.png)

When you clicked it, you will then be directly requested to log in using your ThreeFold Connect app.

## Log in using ThreeFold Connect App

The deployed version comes with a very easy login using the two-factor authentied login using the ThreeFold Connect app.

Fill in the ThreeFold / 3Bot ID that you created. 

![](img/evdc_tfc_login.png)

Press `Sign In`. You will see a screen with an emoji and a corresponding one on your mobile device. Type your password on your smartphone, or authentify yourself with the biometrics credentials in the app. And click on the emoji that matches the emoji on the login screen on your computer.

![](img/evdc_tfc_sso.png)

You're ready to build and configure your Continuous Integration scenarios into ZeroCI !

![](img/evdc_zeroci_05_loggedin.png)


## Accessing Your Deployed Solution

To find and access the ZeroCI server you just deployed, simply go to your eVDC Admin Panel home and find the ZeroCI Widget. Click on **My Workloads** to go to the list of your successfully deployed ZeroCI instance.

![](img/evdc_zeroci_06_myworkload.png)

You can now click the link to go to your deployed ZeroCI.

![](img/evdc_zeroci_07_access.png) 