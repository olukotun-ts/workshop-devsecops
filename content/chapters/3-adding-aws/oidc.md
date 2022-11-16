---
title: "OpenID Connect"
weight: 3
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---
__TIP:__ What is OIDC? Why use it?
Add a context to the job
  - what is a context?

Set up OIDC
In AWS, navigate to the [IAM console](https://console.aws.amazon.com/iam/).

![Navigate to the IAM console](/images/chapter3/_shared/go-to-iam.gif)

In the navigation pane on the left side of the screen, click __Identity providers__.

![Go to Identity providers](/images/chapter3/oidc/2-go-to-idp.gif)

In the next window, click __Add provider__.

![Go to Add providers](/images/chapter3/oidc/3-go-to-add-idp.gif)

To configure the provider, start by selecting the option for __OpenID Connect__.

![Select OpenID Connect](/images/chapter3/oidc/4-select-oidc.gif)

The provider URL is in this format: https<no-hyperlink>://oidc.circleci.com/org/ORGANIZATION_ID, where ORGANIZATION_ID refers to the organization you used to sign in to CircleCI. To obtain this value,
1. Switch to the CircleCI app.
1. In the navigation pane on the left of the screen, click __Organization Settings__.
1. On the next page, copy __Organization ID__ from the __Overview__ section.

![Get your organization ID](/images/chapter3/oidc/5-get-org-id.gif)

Back in the AWS window, add the provider URL with your updated ORGANIZATION_ID and click __Get thumbprint__.

In the field for __Audience__, enter your ORGANIZATION_ID.

Scroll to the bottom of the page and click __Add provider__.

Resources:
- [Contexts](https://circleci.com/docs/contexts)
- [Using OpenID Connect Tokens in Jobs
](https://circleci.com/docs/openid-connect-tokens)
