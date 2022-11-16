---
title: "ECR"
weight: 2
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---
To create an ECR repo for your images, navigate to the ECR dashboard in the AWS console.

![Navigate to the ECR dashboard](/images/chapter3/ecr/1-go-to-ecr.gif)

In the ECR dashboard, click __Create repository__.

![Navigate to the Create repo page](/images/chapter3/ecr/2-go-to-create-repo.gif)

On the _Create repository_ page, enter a name for the repository.

![Name the repository](/images/chapter3/ecr/3-name-repo.gif)

After naming the repository, scroll down to the section titled __Image scan settings__ and click the toggle to enable __Scan on push__.

__TIP__: Configuring registry-level scan settings.

![Enable scan on push](/images/chapter3/ecr/4-enable-scan-on-push.gif)

At the bottom of the page, click on the button to __Create repository__.

![Create the repository](/images/chapter3/ecr/5-create-repo.gif)
