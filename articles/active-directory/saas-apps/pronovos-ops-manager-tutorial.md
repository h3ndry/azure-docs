---
title: 'Tutorial: Azure Active Directory integration with ProNovos Ops Manager | Microsoft Docs'
description: Learn how to configure single sign-on between Azure Active Directory and ProNovos Ops Manager.
services: active-directory
author: jeevansd
manager: CelesteDG
ms.reviewer: celested
ms.service: active-directory
ms.subservice: saas-app-tutorial
ms.workload: identity
ms.topic: tutorial
ms.date: 07/18/2019
ms.author: jeedes
---

# Tutorial: Integrate ProNovos Ops Manager with Azure Active Directory

In this tutorial, you'll learn how to integrate ProNovos Ops Manager with Azure Active Directory (Azure AD). When you integrate ProNovos Ops Manager with Azure AD, you can:

* Control in Azure AD who has access to ProNovos Ops Manager.
* Enable your users to be automatically signed-in to ProNovos Ops Manager with their Azure AD accounts.
* Manage your accounts in one central location - the Azure portal.

To learn more about SaaS app integration with Azure AD, see [What is application access and single sign-on with Azure Active Directory](../manage-apps/what-is-single-sign-on.md).

## Prerequisites

To get started, you need the following items:

* An Azure AD subscription. If you don't have a subscription, you can get a [free account](https://azure.microsoft.com/free/).
* ProNovos Ops Manager single sign-on (SSO) enabled subscription.

## Scenario description

In this tutorial, you configure and test Azure AD SSO in a test environment.

* ProNovos Ops Manager supports **SP and IDP** initiated SSO

## Adding ProNovos Ops Manager from the gallery

To configure the integration of ProNovos Ops Manager into Azure AD, you need to add ProNovos Ops Manager from the gallery to your list of managed SaaS apps.

1. Sign in to the [Azure portal](https://portal.azure.com) using either a work or school account, or a personal Microsoft account.
1. On the left navigation pane, select the **Azure Active Directory** service.
1. Navigate to **Enterprise Applications** and then select **All Applications**.
1. To add new application, select **New application**.
1. In the **Add from the gallery** section, type **ProNovos Ops Manager** in the search box.
1. Select **ProNovos Ops Manager** from results panel and then add the app. Wait a few seconds while the app is added to your tenant.


## Configure and test Azure AD single sign-on

Configure and test Azure AD SSO with ProNovos Ops Manager using a test user called **B.Simon**. For SSO to work, you need to establish a link relationship between an Azure AD user and the related user in ProNovos Ops Manager.

To configure and test Azure AD SSO with ProNovos Ops Manager, complete the following building blocks:

1. **[Configure Azure AD SSO](#configure-azure-ad-sso)** - to enable your users to use this feature.
2. **[Configure ProNovos Ops Manager SSO](#configure-pronovos-ops-manager-sso)** - to configure the Single Sign-On settings on application side.
3. **[Create an Azure AD test user](#create-an-azure-ad-test-user)** - to test Azure AD single sign-on with B.Simon.
4. **[Assign the Azure AD test user](#assign-the-azure-ad-test-user)** - to enable B.Simon to use Azure AD single sign-on.
5. **[Create ProNovos Ops Manager test user](#create-pronovos-ops-manager-test-user)** - to have a counterpart of B.Simon in ProNovos Ops Manager that is linked to the Azure AD representation of user.
6. **[Test SSO](#test-sso)** - to verify whether the configuration works.

### Configure Azure AD SSO

Follow these steps to enable Azure AD SSO in the Azure portal.

1. In the [Azure portal](https://portal.azure.com/), on the **ProNovos Ops Manager** application integration page, find the **Manage** section and select **Single sign-on**.
1. On the **Select a Single sign-on method** page, select **SAML**.
1. On the **Set up Single Sign-On with SAML** page, click the edit/pen icon for **Basic SAML Configuration** to edit the settings.

   ![Edit Basic SAML Configuration](common/edit-urls.png)

1. On the **Basic SAML Configuration** section the application is pre-configured in **IDP** initiated mode and the necessary URLs are already pre-populated with Azure. The user needs to save the configuration by clicking the **Save** button.

1. Click **Set additional URLs** and perform the following step if you wish to configure the application in **SP** initiated mode:

    In the **Sign-on URL** text box, type a URL:
    `https://gly.smartsubz.com/saml2/acs`


4. On the **Set up Single Sign-On with SAML** page, in the **SAML Signing Certificate** section,  find **Certificate (Raw)** and select **Download** to download the certificate and save it on your computer.

	![The Certificate download link](common/certificateraw.png)

6. On the **Set up ProNovos Ops Manager** section, copy the appropriate URL(s) based on your requirement.

	![Copy configuration URLs](common/copy-configuration-urls.png)

### Configure ProNovos Ops Manager SSO

To configure single sign-on on **ProNovos Ops Manager** side, you need to send the downloaded **Certificate (Raw)** and appropriate copied URLs from Azure portal to [ProNovos Ops Manager support team](mailto:support@pronovos.com). They set this setting to have the SAML SSO connection set properly on both sides.
### Create an Azure AD test user

In this section, you'll create a test user in the Azure portal called B.Simon.

1. From the left pane in the Azure portal, select **Azure Active Directory**, select **Users**, and then select **All users**.
1. Select **New user** at the top of the screen.
1. In the **User** properties, follow these steps:
   1. In the **Name** field, enter `B.Simon`.  
   1. In the **User name** field, enter the username@companydomain.extension. For example, `B.Simon@contoso.com`.
   1. Select the **Show password** check box, and then write down the value that's displayed in the **Password** box.
   1. Click **Create**.

### Assign the Azure AD test user

In this section, you'll enable B.Simon to use Azure single sign-on by granting access to ProNovos Ops Manager.

1. In the Azure portal, select **Enterprise Applications**, and then select **All applications**.
1. In the applications list, select **ProNovos Ops Manager**.
1. In the app's overview page, find the **Manage** section and select **Users and groups**.

   ![The "Users and groups" link](common/users-groups-blade.png)

1. Select **Add user**, then select **Users and groups** in the **Add Assignment** dialog.

	![The Add User link](common/add-assign-user.png)

1. In the **Users and groups** dialog, select **B.Simon** from the Users list, then click the **Select** button at the bottom of the screen.
1. If you're expecting any role value in the SAML assertion, in the **Select Role** dialog, select the appropriate role for the user from the list and then click the **Select** button at the bottom of the screen.
1. In the **Add Assignment** dialog, click the **Assign** button.

### Create ProNovos Ops Manager test user

In this section, you create a user called B.Simon in ProNovos Ops Manager. Work with [ProNovos Ops Manager support team](mailto:support@pronovos.com) to add the users in the ProNovos Ops Manager platform. Users must be created and activated before you use single sign-on.

### Test SSO 

In this section, you test your Azure AD single sign-on configuration using the Access Panel.

When you click the ProNovos Ops Manager tile in the Access Panel, you should be automatically signed in to the ProNovos Ops Manager for which you set up SSO. For more information about the Access Panel, see [Introduction to the Access Panel](https://support.microsoft.com/account-billing/sign-in-and-start-apps-from-the-my-apps-portal-2f3b1bae-0e5a-4a86-a33e-876fbd2a4510).

## Additional Resources

- [ List of Tutorials on How to Integrate SaaS Apps with Azure Active Directory ](./tutorial-list.md)

- [What is application access and single sign-on with Azure Active Directory? ](../manage-apps/what-is-single-sign-on.md)

- [What is conditional access in Azure Active Directory?](../conditional-access/overview.md)