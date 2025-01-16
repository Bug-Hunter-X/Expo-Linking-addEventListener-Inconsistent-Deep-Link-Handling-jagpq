# Expo Linking.addEventListener Inconsistent Deep Link Handling

This repository demonstrates an issue with Expo's `Linking.addEventListener` API where deep link handling is unreliable when the app is in the background.  The issue manifests as deep links sometimes being missed, even though the event listener is correctly set up.

## Problem

The `Linking.addEventListener` method is used to listen for deep links.  However, when the app is already running in the background and a deep link is opened, the listener does not always fire as expected. This inconsistency creates unreliable behavior in handling deep links.

## Solution

This issue is still under investigation in the Expo ecosystem.  A workaround may include using a more robust deep linking solution (such as Firebase Dynamic Links) which provides more reliable background handling.