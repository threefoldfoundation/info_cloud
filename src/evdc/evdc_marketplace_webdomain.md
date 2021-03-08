# Deploy a solution under your webdomain

A solution can be deployed under an auto-generated url or can be linked to your own domain. 

## How to link a marketplace solution to your own domain ? 

During the chatflow, the question will be asked to select a subdomain. Select the option `Choose a custom subdomain`to publish your solution to your own domain.

![](img/evdc_mktpl_domain_01_custom.png)

Now, you need to link the domain name to the IP address that is reserved with your VDC. To do so, first copy the IP address. 

![](img/evdc_mktpl_domain_02_copyip.png)

Then make the link between the IP and the domain name in a domain name registry. 

![](img/evdc_mktpl_domain_03_linkip.png)

Now your domain name is linked to the IP address. You can check this using the`nslookup`command. 

![](img/evdc_mktpl_domain_05_checkdomain.png)

Enter now this domain name in the the chatflow.

![](img/evdc_mktpl_domain_06_pastedomain.png)

This will result in a deployment that is immediately accessible using the chosen domain name!

![](img/evdc_mktpl_domain_07_success.png)

You can check right away. 

![](img/evdc_mktpl_domain_08_checkurl.png)

Also in your list of deployed solutions, you can now easily find back and visit the deployed solution through the chosen url. 

![](img/evdc_mktpl_domain_09_findsolution.png)


