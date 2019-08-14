> Quick reference for all MEH tools out there!

# Sitemap

* [Edje](#edje)
* [Hostifier](#hostifier)
* [Richifier](#richifier)
* [Staticifier](#staticifier)
* [Scalifier](#scalifier)
* [Clicktrackifier](#clicktrackifier)
* [LemonPI feed importer](#lemonpifeedimporter)
* [DOOH-ifier](#dooh-ifier)
* [GSP-ifier](#gsp-ifier)
* [Anna](#anna)
* [In-App tester](#inapptester)
* [Creating a Contentful model for LemonPI](#contentfulforlemonpi)
* [Template Campaign Laucher (coming soon)](#templatecampaignlauncher)
* [Manage Manager](#managemanager)
* [Mobile Wall](#mobilewall)
* [Celtra-AppNexus Parser](#celtraappnexusparser)
* [Temporary Uploader](#temporaryuploader)
* [Wrike ID redirect page](#wrikeidredirect)
* [Optinoud](#optinoud)

## <a name="edje"></a>[Edje](http://edje.greenhousegroup.com)

The MVP for a creative workflow platform, so we can easily send (dynamic) previews of creative material to clients and gather their feedback. It has a smooth integration with Wrike so it doesn’t feel like ‘yet another platform’.

### How to use

You can only use Edje through Wrike. In order to extend Wrike for the use with Edje, you need to install [CJS for Chrome](https://chrome.google.com/webstore/detail/custom-javascript-for-web/poakhlngfciodnhlhhgnaaelnpjljija) first. Afterwards, visit Wrike (in your browser, not the app) and click the blue **cjs** button in the top right corner. Then paste the following script in the textarea:

```js
var e=document.createElement('script');e.src='https://s3.eu-central-1.amazonaws.com/ghg-tools/ghg-edje/wrike-edje.js',document.body.appendChild(e);
```

Press **save**.

Done! You should now see an 'Add creative' button to every task in Wrike. In order to integrate LemonPI bannersets, please also install the [Manage Manager](https://meh.greenhousegroup.com/#manage-manager).

## <a name="hostifier"></a>[Hostifier](https://hostifier.meh.greenhousegroup.com)

Web app for hosting static assets on cdn.greenhousegroup.com

## <a name="richifier"></a>[Richifier](https://ghg-richifier-live.herokuapp.com/)

This will add the chosen rich media template to your LemonPI Studio creative zip, which makes it compatible to upload to Weborama.

## <a name="staticifier"></a>[Staticifier](https://ghg-staticifier-live.herokuapp.com/)

When using LemonPI to export creatives to a DSP is not an option, you can use the Staticifier to strip all Greenhouse Group related dependencies from a LemonPI Studio creative zip. This makes it suitable to deliver creatives to agencies that want to serve these without LemonPI.

## <a name="scalifier"></a>[Scalifier](https://ch-scalifier.herokuapp.com/)

The Scalifier allows for super-fast resizing of creatives. Even though it sounds like a minor task, it actually circumvents many mundane manual steps which quickly add up in hours.

## <a name="clicktrackifier"></a>[Clicktrackifier](http://clicktrackifier.greenhousegroup.com/)

The Cicktrackifier enables a clicktracker per size in LemonPI Manage.

## <a name="lemonpifeedimporter"></a>[LemonPI Feed Importer](https://ghg-lemonpi-feed-import-live.herokuapp.com)

Use your LemonPI account to import product feeds, and use them as a Smart Pixel Dynamic Input.

## <a name="dooh-ifier"></a>[DOOH-ifier](https://ch-doohifier.herokuapp.com/)

DOOH-ifier is a webapp for Creative Hub to make initialised LemonPI Studio-creatives for DOOH from the required screen specifications.

## <a name="gsp-ifier"></a>[GSP-ifier](https://meh-gspifier.herokuapp.com/)

Generate single-image GSPs on the fly.

## <a name="anna"></a>Anna

Create off-site A/B tests through Wrike. Add and tick the "Off-site test" custom field in your Wrike task, and fill in the following custom fields: "Default Line Item ID", "Variant 1 Line Item ID", "Q-impression Pixel ID", "Transaction Pixel ID". Then and change the task's workflow status to "Live". Anna will report and notify you about any test data significance.

## <a name="inapptester"></a>[In-app Tester](https://meh-inapp-testing.herokuapp.com/add.html)

Makes in-app testing of LemonPI creatives flawless.

## <a name="contentfulforlemonpi"></a>[Creating a Contentful model for LemonPI](https://docs.google.com/document/d/1Vyn5wKO7TH-lTXwbSnN6HNNGjJHsFE5hFlch81AMkO4/edit)

This guide explains how you can create and configure a new Contentful model for usage with LemonPI (Smart LemonPI Pixel dynamic input).

## <a name="templatecampaignlauncher"></a>[The Campaign Laucher (TCL)](http://tcl.meh.greenhousegroup.com)

Platform to launch PBU campaigns fast and easy.

## <a name="managemanager"></a>Manage Manager

Adds some improvements on top of LemonPI Manage, like cloning a dynamic input.

### How to use

To use the Manage Manager, you need to install [CJS for Chrome](https://chrome.google.com/webstore/detail/custom-javascript-for-web/poakhlngfciodnhlhhgnaaelnpjljija) first. Afterwards, visit manage.lemonpi.io and click the blue **cjs** button in the top right corner. Then paste the following script in the textarea:

```js
var e=document.createElement('script');e.src='https://cdn.greenhousegroup.com/ghg-nl/manage-manager/script.js',document.body.appendChild(e);
```

Press **save**.

Done!

## <a name="mobilewall"></a>[Mobile Wall](https://bit.ly/bmiwall2)

Quickly open URLs on other devices by using the Mobile Wall.

## <a name="celtraappnexusparser"></a>[Celtra-AppNexus parser](https://meh-celtra-appnexus-parser.herokuapp.com/)

For Unilever, the (huge amount) creatives have to be built in Celtra, but we want to run the creatives in AppNexus. Because there is no 1-to-1 integration, the specialist had to manually import the Celtra tags in AppNexus. We created an easy converter that changed a 2-hour job to a 2-minute job.

## <a name="temporaryuploader"></a>[Temporary Uploader](https://ghg-temporary-uploader.herokuapp.com/)

When using external assets like videos or images in display, you need URLs while developing. The Temporary Uploader will do just that. (ask a MEHmber for the password)

## <a name="wrikeidredirect"></a>[Wrike ID redirect page](https://wrike.greenhousegroup.com/)

Quickly open a Wrike task from a Wrike ID, like "CZ-123".

## <a name="optinoud"></a>[Optinoud](https://www.npmjs.com/package/generator-optinoud)

Optinoud lets you write ES6+ and SASS snippets, while transpiling to ES5+CSS, and live injecting it into a specified website.
