---
title: "OIDC Role"
weight: 1
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---
# Create an IAM Role

From the IAM dashboard, navigate to the _Create role_ page by clicking __Roles__ in the navigation pane then clicking the __Create role__ button.

![Navigate to the Create role page](/images/chapter3/_shared/go-to-create-role.gif)

In the section titled _Trusted entity type_, select __Web identity__; and in the section titled __Web identity__, use the dropdown menu to select the IdP you created in the preceding section.

![Select an IdP](/images/chapter3/roles-permissions/oidc/2-select-idp.gif)

After selecting an IdP, use the __Audience__ dropdown menu to select the audience you added in the preceding section. Then click __Next__.

![Select IdP audience](/images/chapter3/roles-permissions/oidc/3-select-audience.gif)

# Add Permissions
Next, you will add permissions to grant access to ECR and EKS. Type ECR in the search bar and select ...

![Add ECR permissions](/images/chapter3/roles-permissions/oidc/4-add-ecr-permissions.gif)


Next, type EKS in the search bar. Select the _AmazonEKSCluster_ policy. Scroll to the bottom of the page and click __Next__.

![Add EKS permissions](/images/chapter3/roles-permissions/oidc/5-add-eks-permissions.gif)

Finally, give the role a descriptive name; then click __Create role__.

![Create role](/images/chapter3/roles-permissions/oidc/6-name-role.gif)

Resources:
- IAM roles and permissions
- least-privilege