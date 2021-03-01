# Host a Blog on TF Grid via eVDC

By using eVDC you can easily deploy and host your own blog on top of the ThreeFold_Grid.

![](img/evdc_blog_06_url.png)

## Requirements

- A **github account**.
- A **public github repository** complete with folders containing your blog codes and files. [**Click here**](https://github.com/threefoldtech/blog_example) to see an example of a blog repo that you can fork (copy to your own github).
- **Optional for custom domain**: an active domain that assigns to a particular IP that will be given to you during deployment. Depending where you purchased your domain, each domain registery has its own procedure on how to assign an IP. Click [**here**](https://www.hostmysite.com/support/cpanel/dns/domain_point/) to read a general tutorial on how to assign an IP to your domain.
- An **active eVDC** with sufficient capacity.

## Get Started

Once you're logged in the eVDC, find the **Blog** marketplace widget on your admin panel and click on **Deploy** button.

![](img/evdc_marketplace_blog_widget.png)

Create a name for your blog. This name will be used to identify your deployment on your 'Deployed Solutions' list.

![](img/evdc_blog_01_name.png)

Select the domain type for your blog. For deployment with random subdomain, select `Choose subdomain for me on a gateway`. For deployment with a particular available subdomain, select `Choose a custom subdomain on a gateway`. To host a blog using your own domain, select `choose a custom domain`.

![](img/evdc_blog_02_domain.png)

Select the vdc capacity plan for your blog usage.

![](img/evdc_blog_03_config.png)

Add your blog repository files to the deployment.

![](img/evdc_blog_04_configuration.png)

- Repository url: the url address of your blog's source codes on github
- Branch: the main official working version of your project. Read more about github branch [here](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-branches)
- Source directory: the name of the main folder in your github repository where all your html codes, css, index.html page, and other codes that make up your blog pages live.

To create a blog from a template website from ThreeFold, go to [Template Website](https://github.com/threefoldtech/blog_example) on github and click on fork.

![](img/evdc_blog_07_fork.png)

Go to your newly forked github repository and copy the Repository url on your forked repository

![](img/evdc_blog_08_repo_copy.png)

Paste the url to the chatflow 'Repository url' form.

Identify the branch of your website (ex. `main` ), identify the main source folder of your website and click `Next`.

![](img/evdc_blog_04_configuration.png)

Now the VDC has all what is needed to deploy your blog.

Congratulations! you just successfully hosted a website on the ThreeFold_Grid!
![](img/evdc_blog_05_success.png)

Click on the domain to open and preview your newly hosted blog.

![](img/evdc_blog_06_url.png)

Update and complete your blog in the forked template on Github. Evidently, you can customize your blog content after it's deployed. Always remember which Github repo you are using, and happy writing !