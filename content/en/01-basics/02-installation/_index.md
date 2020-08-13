+++
title = "Installation"
weight = 010200
chapter = false
pre = "<b>b. </b>"
disableToc = false
+++

The following steps will help you to install and setup the template for your workshop.

## 1. Download the template

Click in the following link to download a skeleton project of the template:

- [AWS Workshop project skeleton](https://github.com/falej/aws-workshop-hugo-template/archive/master.zip)

## 2. Setup the template

1. Unzip the file downloaded. It will unzip a folder with the template skeleton
2. Rename the unziped folder with the name of your project. For example: `awsome-workshop`

## 3. Test the template

1. **cd** to your project folder. For example: `cd awsome-workshop`
2. Run `hugo server -p 8080`
3. Open a browser and go to [http://localhost:8080](http://localhost:8080).

{{% notice warning %}}
If you didn't install Hugo, the step 2 will throw an error because the command is not recognized.
{{% /notice %}}

A page like below should be displayed:

![IMG001](/images/01-basics/02-installation/IMG001.png?classes=border)

Congratulations! You can start to create the content of your workshop.
