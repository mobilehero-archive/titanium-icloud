# @titanium/icloud

[![@titanium/icloud](https://img.shields.io/npm/v/@titanium/icloud.png)](https://www.npmjs.com/package/@titanium/icloud)


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
* [Usage](#usage)
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

* [x] Includes Titanium native iOS module: `ti.icloud 1.1.0`


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

## Usage
See `example/app.js`.

## Author
Matthew Apperson, Hans Knöchel

## Module History
View the [change log](./documentation/changelog.md) for this module.


## 📚Learn More

- [ti.icloud GitHub Repo](https://github.com/appcelerator-modules/ti.icloud) - Repo for original ti.icloud module


## 📣 Feedback

Have an idea or a comment?  [Join in the conversation here](https://github.com/brentonhouse/ti.icloud/issues)! 

## ©️ Legal

Modules are licensed under Apache 2.0 from https://github.com/appcelerator-modules/ti.icloud

Alloy is developed by Appcelerator and the community and is Copyright © 2012-Present by Appcelerator, Inc. All Rights Reserved.

Alloy is made available under the Apache Public License, version 2. See their license file for more information.

Appcelerator is a registered trademark of Appcelerator, Inc. Titanium is a registered trademark of Appcelerator, Inc. Please see the LEGAL information about using trademarks, privacy policy, terms of usage and other legal information at http://www.appcelerator.com/legal.