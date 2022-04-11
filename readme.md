[//]: # (header-start)

<h1 align="center">
	<a href="https://blog.axway.com/mobile-apps/changes-to-application-development-services">
		Preparing for end of Axway
	</a>	
</h1>
<h2 align="center">
	👇 &nbsp; support for Amplify Cloud and Mobile   &nbsp; 👇
</h2>	

<a href="https://brenton.house/saying-goodbye-to-axway-amplify-titanium-31a44f3671de">
	<p align="center">
		<img src="https://cdn.secure-api.org/images/RIP-Axway-Amplify-Titanium.png" alt="RIP Axway Amplify Titanium (2010 - 2022)" width="80%" />
	</p>
</a>	
<p align="center">
	<a href="https://blog.axway.com/mobile-apps/changes-to-application-development-services">
			🪦 &nbsp; RIP Axway Amplify Titanium (2010 - 2022)
	</a>
</p>
<p align="center">
	<a href="https://blog.axway.com/mobile-apps/prepare-your-apps-for-appcelerator-end-of-support">
			🪦 &nbsp; RIP Axway Amplify Cloud Services (2012 - 2022)
	</a>
</p>
<p align="center">
	<a href="https://blog.axway.com/mobile-apps/prepare-your-apps-for-appcelerator-end-of-support">
			🪦 &nbsp; RIP Axway Amplify Crash Analytics (2015 - 2022)
	</a>
</p>

<hr>
<h4 align="center">
🛑 &nbsp;&nbsp; <a href="https://blog.axway.com/mobile-apps/prepare-your-apps-for-appcelerator-end-of-support">Axway support for Amplify products has ended</a> for most products related to mobile and cloud. 
</h4>

<h4 align="center">
A few of the open-source versions of Axway Amplify products will live on after <a href="">Axway Amplify End-of-Life</a> (EOL) announcements.  However, all closed-source projects and most open-source projects are now dead.  
	</h4>

<p>&nbsp;</p>

> 👉 &nbsp;&nbsp; A group of Axway employees, ex-Axway employees, and some developers from Titanium community have created a legal org and now officially decide all matters related to future of these products.  

<p>&nbsp;</p>
<hr>


## API FAQ:

* [API Best Practices](https://brenton.house)
* [What is API Security?](https://brenton.house/what-is-api-security-5ca8117d4911)
* [OWASP Top 10 List for API Security](https://www.youtube.com/watch?v=GLVHDj0Cpg4)
* [What is API Security?](https://brenton.house/what-is-api-security-5ca8117d4911)
* [Top API Trends for 2022](https://brenton.house/top-10-api-integration-trends-for-2022-49b05f2ef299)
* [What is a Frankenstein API?](https://brenton.house/what-is-a-frankenstein-api-4d6e59fca6)
* [What is a Zombie API?](https://brenton.house/what-is-a-zombie-api-6e5427c39b6a)
* [API Developer Experience](https://brenton.house/keys-to-winning-with-an-awesome-api-developer-experience-62dd2fa668f4)
* [API Cybersecurity 101](https://brenton.house/what-is-api-security-5ca8117d4911)
* [YouTube API Videos](https://youtube.com/brentonhouse)
* [YouTube API Shorts Videos](https://youtube.com/apishorts)

&nbsp;

[![Click to watch on Youtube](https://img.youtube.com/vi/GLVHDj0Cpg4/0.jpg)](https://www.youtube.com/watch?v=GLVHDj0Cpg4&list=PLsy9MwYlG1pew6sktCAIFD5tbrXy9HUQ7  "Click to watch on YouTube")


> &nbsp; [↑ Watch video on YouTube ↑](https://www.youtube.com/watch?v=GLVHDj0Cpg4&list=PLsy9MwYlG1pew6sktCAIFD5tbrXy9HUQ7)

&nbsp;



<p>&nbsp;</p>
<hr>

<p>&nbsp;</p>
<p>&nbsp;</p>

[//]: # (header-end)




# @titanium/icloud

[![@titanium/icloud](https://img.shields.io/npm/v/@titanium/icloud.png)](https://www.npmjs.com/package/@titanium/icloud)
[![Dependabot Status](https://api.dependabot.com/badges/status?host=github&repo=brentonhouse/titanium-icloud)](https://dependabot.com)


> Native module that allows you to use the Apple iCloud framework with Axway Titanium native mobile apps.

* [📝 Description](#-description)
* [🚀 Getting Started](#-getting-started)
	* [Install `@titanium/icloud` in root of project](#install-titaniumicloud-in-root-of-project)
* [Requirements](#requirements)
* [✨Features](#features)
* [Example](#example)
* [Methods](#methods)
	* [`bool sync()`](#bool-sync)
	* [`void setString(string key, string value)`](#void-setstringstring-key-string-value)
	* [`void setBool(string key, bool value)`](#void-setboolstring-key-bool-value)
	* [`void setDictionary(string key, dictionary value)`](#void-setdictionarystring-key-dictionary-value)
	* [`void setList(string key, object[] value)`](#void-setliststring-key-object-value)
	* [`void setInt(string key, int value)`](#void-setintstring-key-int-value)
	* [`void setDouble(string key, double value)`](#void-setdoublestring-key-double-value)
	* [`void setObject(string key, object value)`](#void-setobjectstring-key-object-value)
	* [`string getString(string key)`](#string-getstringstring-key)
	* [`bool getBool(string key)`](#bool-getboolstring-key)
	* [`dictionary getDictionary(string key)`](#dictionary-getdictionarystring-key)
	* [`object[] getList(string key)`](#object-getliststring-key)
	* [`int getInt(string key)`](#int-getintstring-key)
	* [`double getDouble(string key)`](#double-getdoublestring-key)
	* [`object getObject(string key)`](#object-getobjectstring-key)
	* [`dictionary getAll()`](#dictionary-getall)
	* [`void remove(string key)`](#void-removestring-key)
* [Events](#events)
	* [externalChange](#externalchange)
	* [needsInitialSync](#needsinitialsync)
	* [quotaViolated](#quotaviolated)
	* [accountChange](#accountchange)
* [Author](#author)
* [Module History](#module-history)
* [📚Learn More](#learn-more)
* [📣 Feedback](#-feedback)
* [©️ Legal](#️-legal)


## 📝 Description

This is a repackaging of the compiled iOS module for [ti.icloud](https://github.com/appcelerator-modules/ti.icloud) to allow for installation via npm.

## 🚀 Getting Started

### Install `@titanium/icloud` in root of project

```bash
npm install @titanium/icloud
```

## Requirements

There are several requirements for this module to function properly:

- [x] This module will ONLY work with iOS 5 devices and higher. THE SIMULATOR WILL NOT WORK!
- [x] All provisioning profiles must have been generated from an application configured to support iCloud. Check in your Provisioning Portal - [x] App IDs that the "iCloud" column says "Enabled" beside your app.
- [x] The device must be set up to use iCloud, and be signed in to an iCloud account.

Otherwise, you will receive warnings, and any calls to the "sync" method will return false.

If you have met the above requirements and you are still receiving errors, try removing the profiles from your device, and delete them from your Apple account. Regenerate them and try again.


## ✨Features

* [x] Includes Titanium native iOS module: `ti.icloud 2.0.0`


## Example

This module was designed to follow a similar scheme like Ti.Facebook and Ti.GoogleSignIn.

```js
const icloud = require('@titanium/icloud');
```



## Methods

### `bool sync()`

Forces your recent property changes to be saved to disk. Calling this method is optional, and it does not influence
when Apple chooses to synchronize your changes with their servers and other iOS devices.

### `void setString(string key, string value)`

Stores a string.

### `void setBool(string key, bool value)`

Stores a boolean.

### `void setDictionary(string key, dictionary value)`
Stores a dictionary of any serializable values.

### `void setList(string key, object[] value)`

Stores an array of serializable values.

### `void setInt(string key, int value)`

Stores an integer.

### `void setDouble(string key, double value)`

Stores a double.

### `void setObject(string key, object value)`

Stores a serializable object.

### `string getString(string key)`

Retrieves a previously stored string.

### `bool getBool(string key)`

Retrieves a previously stored boolean.

### `dictionary getDictionary(string key)`

Retrieves a previously stored dictionary.

### `object[] getList(string key)`

Retrieves a previously stored array.

### `int getInt(string key)`
Retrieves a previously stored integer.

### `double getDouble(string key)`

Retrieves a previously stored double.

### `object getObject(string key)`

Retrieves a previously stored object.

### `dictionary getAll()`

Retrieves all previously stored properties as a dictionary. The key you stored the property with will be its key in the dictionary.

### `void remove(string key)`

Removes a previously stored property permanently.


## Events

### externalChange

The value changed on the remote server. This can occur when another device syncs a new value to the server.

Receives a dictionary with the following keys:

* keys (`[String]`): Affected store keys.

### needsInitialSync

Local changes were discarded because an initial sync from the server has not yet happened. Initial syncs happen the
first time the device is synced but may also happen when user account settings change.

Receives a dictionary with the following keys:

* keys (`[String]`): Affected store keys.

### quotaViolated

The key-value store has exceeded its space quota on the server.

Receives a dictionary with the following keys:

* keys (`[String]`): Affected store keys.

### accountChange

The user has changed the primary iCloud account.
The keys and values in the local key-value store have been replaced with those from the new account, regardless
of the relative timestamps.

Receives a dictionary with the following keys:

* keys (`[String]`): Affected store keys.


## Author
Matthew Apperson, Hans Knöchel

## Module History
View the [change log](./changelog.md) for this module.


## 📚Learn More

- [ti.icloud GitHub Repo](https://github.com/appcelerator-modules/ti.icloud) - Repo for original ti.icloud module


## 📣 Feedback

Have an idea or a comment?  [Join in the conversation here](https://github.com/brentonhouse/titanium-icloud/issues)! 

## ©️ Legal

Modules are licensed under Apache 2.0 from https://github.com/appcelerator-modules/ti.icloud

Alloy is developed by Appcelerator and the community and is Copyright © 2012-Present by Appcelerator, Inc. All Rights Reserved.

Alloy is made available under the Apache Public License, version 2. See their license file for more information.

Appcelerator is a registered trademark of Appcelerator, Inc. Titanium is a registered trademark of Appcelerator, Inc. Please see the LEGAL information about using trademarks, privacy policy, terms of usage and other legal information at http://www.appcelerator.com/legal.