# Deploy Cryptpad in your VDC

[Cryptpad](https://cryptpad.fr/) is a private-by-design alternative to the Office tools als offered by Microsoft and Google. 
It has most of the same crucial functionalities you would be used to with existing tools.
However, all the content stored on CryptPad is encrypted before being sent, which means nobody can access your data unless you give them the keys (not even us).
Encryption happens in the browser that is used to access the "pads" – and therefore the central storage facility used does not see un-encrypted data and only sees encrypted data passing by.

### Getting Started

In the marketplace, click on the `DEPLOY` button. 

![](img/evdc_marketplace_cryptpad_widget.png)

Give your solution a name.

![](img/evdc_cryptpad_01_name.png)

You can choose to create a url which is part of your domain, or have one auto-generated. 

![](img/evdc_cryptpad_02_domain.png) 

Choose the size of the capacity that you want to reserve for this solution. 
![](img/evdc_cryptpad_03_flavour.png)

Now all info is available to create your Cryptpad environment. The url that gives access to it can be found on the next screen, or in the deployed solutions overview.

![](img/evdc_cryptpad_05_success.png)


Now all what remains to be done, is the configuration of your Cryptpad instance.

### Login using ThreeFold Connect App

Login can be done through e-mail access but also using the ThreeFold Connect App 2-factor authentication. 

![](img/evdc_cryptpad_06_url.png)

Click on `Threefold Connect`, fill in your Threefold/3Bot ID and use the Threefold Connect app on your mobile device to tap the corresponding emoji. 

![](img/evdc_tfc_login.png)
![](img/evdc_tfc_sso.png)

Once you've done that, you're connected and you can start creating and sharing your private documents. 

![](img/evdc_cryptpad_09_runs.png)