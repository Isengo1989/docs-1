# Quality Guidelines for the Plugin System in the Shopware Store

> **Changelog**
>
>> 09/10/24: Quality guidelines for apps in the plugin system.
>
>> 01/08/24: [Added - Message queue](..//quality-guidelines-plugins/#message-queue)
>
>> 06/09/23: [Added - Rules for own composer dependencies](../quality-guidelines-plugins/#own-composer-dependencies)
>
>> 26/07/23: [Added - Identical name rule](../quality-guidelines-plugins/#every-app-based-on-the-plugin-system)

## The way we test apps based on the plugin system

It is always a good idea to review our test process before submitting your app for review.
This ensures the quickest way for your app to be published.

We perform the *first test*, and if successful, we do the *follow-up test* again with the most current Shopware version.

The Shopware installation is located in a subfolder.
It has a language sub-shop/sales channel with a virtual URL as well as an independent sub-shop/sales channel with its own URL, also located in a subfolder.
E.g. `myshop.com/public/admin`.
The app must neither produce any error messages in the administration nor in the frontend.

The app is tested with the latest official Shopware 6 CE Version.

::: info
We always test with the [actual SW6 version](https://www.shopware.com/de/download/#shopware-6).
So set it to the actual SW6 version e.g., shopware/testenv:6.6.6.
Always test with the app`s highest supported Shopware version.
:::

Link: [Test your app for the Shopware Store (DE):](https://www.youtube.com/watch?v=gLb5CmOdi4g) and EN version is coming soon.  

**Progressive Web App:** If your app is PWA compatible and you would like the PWA flag, please contact us at [alliances@shopware.com](mailto:alliances@shopware.com).

## Checklist for app testing

Could you be sure to use the most recent testing checklist from Shopware and not any other provider?
Please pay attention to every point in this guide. We'll review it before you release your app.

### Every app based on the plugin system

* We pay attention to the automatic code review and look for security issues and shopware coding standards in the manual code review.

* We check the complete functionality of the app (separately sales channel configurations in the config.xml, the uninstallation and reinstallation procedure) and check for styling errors on every viewport.

* We want to improve the quality of the Shopware Community Store and offer as many different apps as possible.
Hence, we check for a functional comparison with other apps already in the Shopware Community store, in the Rise edition or above.
If an extension with the same function exists and it does not fit into one of our differentiator clusters, it can be rejected as it doesn't provide any added value.
If you would like more information, please write an email to [qa@shopware.com](mailto:qa@shopware.com).

Link: [Differentiator cluster for Shopware extensions](../../../../../resources/guidelines/testing/Differentiator-Clusters.md)

Link: [Documentation for Extension Partner](https://docs.shopware.com/en/account-en/extension-partner/extensions?category=account-en/extension-partner#how-can-i-request-a-preview)

::: info
**Safe your app idea and get a preview in the store**
If you already have an idea and don't want it to be snatched away, ensure you get it by creating a preview in your account.
You can apply for this if you have maintained placeholder images for the store, meaningful use cases, highlight features, a description, and a release month without uploading any binary.
:::

## App store description

The release to the English store is standard.
As an app will be released in both stores (German and International), the content must accurately translate 1:1 from English to German.

* The mandatory number of characters is set in short and long descriptions. No blank spaces as fillers are allowed (EN/DE).
* Check if the description makes sense and describe the use cases of your app.
* Check if your configuration manual includes step-by-step instructions on how to configure and use your app.
* Check if you have included enough screenshots showing the app in action in the Storefront and administration.
* Check if the display name does not contain the terms "plugin" or "shopware".
* Check if all images for the English store description contain the English language. [Please do not mix English with other languages in your screenshots. Screenshots in German for the German store description are optional.]
* Check if you explained the setup of the app and added a configuration manual.

### Display Name

According to the new naming scheme, extensions may no longer display the words "plugin" and "shopware" in their names.
An extension with a name that directly reflects its functional purpose is permissible, even if it shares the same name as another extension.

Also, the store-display name had to be used for `composer.json` and `config.xml`.

### Short description

(Min. 150 — max. 185 characters)—The app's short description must be unique and at least 150 characters long.
Use the short description wisely, as the text will tease your app in the overview along with the "Customers also bought" and "Customers also viewed" recommendations.
The short description is also published as a meta-description.

### Description

(Min. 200 characters)—The app description must be at least 200 characters long and describe the app's functions in detail.

* Inline styles will be stripped. The following HTML tags are allowed:

```markdown
<a> <p> <br> <b> <strong> <i> <ul> <ol> <li> <h2> <h3> <h4> <h5>
```

* **Tips:**

    * When it comes to increasing your app sales, it is important that potential customers feel completely informed about your products and services.
	To this end, you should provide description, highlights, and features that are meaningful, detailed, and easy to understand, even for people with very minimal technical knowledge.
	Explain step-by-step how your app works and how to use it to achieve the desired result.
	Of course, your app description should be accompanied by clean HTML source code.

    * Video content increases awareness and trust and has proven to convert potential customers better than other content types.
	You can help your customers better understand your app or service with explainer videos, product demos, tutorials, etc.
	You can embed a maximum of 2 YouTube videos in your app description.

::: info
You can no longer advertise your Shopware certificates within the app description, in your app images, or in your manufacturer profile.
The manufacturer/partner certificates are dynamically loaded at the end of each app description and published by us.
:::

### Images

::: info
Screenshots and preview images in English are standard. Only full English screenshots are accepted. Please do not mix English with other languages in your screenshots. Screenshots in German for the German store description are optional.
:::

Include several screenshots and descriptive images from the Storefront and backend that represent the app functionality.
They must show the app "in action", its configuration options, and how to use it.
We recommend uploading screenshots showing the mobile and desktop-view.

Link: [How To - Add images and icons to extensions](https://docs.shopware.com/en/account-en/adding-pictures-and-icons/how-to)

### Link to demoshop

If you provide a demo shop, the link must be valid (the URL cannot contain `http:` or `https:`).
Do not link to your test environments, as we will delete them automatically two weeks after they are created.

### Personal data protection information

If necessary, personal data protection information has to be set.
If personal data of the customers (store operator and/or his customers) are processed with this extension according to Art. 28 DSGVO, the following information of the data processing company must be stored in the field "Subprocessor".

If other companies are involved in the data processing of personal data, the same information must be stored accordingly for them in the field "Further subprocessors".

### Configuration manual

Explain how your app is installed and configured, how it works on a technical base, and how it can be used to achieve the desired result.
Of