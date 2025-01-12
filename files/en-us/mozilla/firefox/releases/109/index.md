---
title: Firefox 109 for developers
slug: Mozilla/Firefox/Releases/109
tags:
  - "109"
  - Firefox
  - Mozilla
  - Release
---

{{FirefoxSidebar}}

This article provides information about the changes in Firefox 109 that will affect developers. Firefox 109 is the current [Nightly version of Firefox](https://www.mozilla.org/en-US/firefox/channel/desktop/#nightly) and will ship on [January 17, 2023](https://wiki.mozilla.org/RapidRelease/Calendar#Future_branch_dates).

## Changes for web developers

### Developer Tools

### HTML

- The {{HTMLElement("input/range", "range")}} element supports [`list`](/en-US/docs/Web/HTML/Element/input/range#list) attribute which links via an id to a {{HTMLElement("datalist")}} to allow Firefox to display tick marks along the range.

#### Removals

### CSS

- The [`<system-color>`](/en-US/docs/Web/CSS/system-color) CSS data type now supports the values [`Mark`](/en-US/docs/Web/CSS/system-color#mark), [`MarkText`](/en-US/docs/Web/CSS/system-color#marktext), and [`ButtonBorder`](/en-US/docs/Web/CSS/system-color#buttonborder) ({{bug(1638052)}}).

#### Removals

### JavaScript

#### Removals

### HTTP

#### Removals

### Security

#### Removals

### APIs

#### DOM

#### Media, WebRTC, and Web Audio

#### Removals

### WebAssembly

#### Removals

### WebDriver conformance (WebDriver BiDi, Marionette)

#### WebDriver BiDi

#### Marionette

## Changes for add-on developers

- Manifest V3 is now supported with the ability to sign and release Manifest V3 extensions on AMO. See the [Manifest v3 signing available November 21 on Firefox Nightly](https://blog.mozilla.org/addons/2022/11/17/manifest-v3-signing-available-november-21-on-firefox-nightly/) blog post for more information.
- The default [Content Security Policy (CSP)](/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy) for Manifest V3 extensions has been updated to [include `upgrade-insecure-requests`](/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy#upgrade_insecure_network_requests_in_manifest_v3). This means that, by default, all network requests are upgraded to use `https:`. Extensions that need to use `http:` can do so by overriding the default CSP using the [`content_security_policy`](/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json/content_security_policy) manifest.json key ({{bug(1797086)}}).

### Removals

### Other

## Older versions

{{Firefox_for_developers(108)}}
