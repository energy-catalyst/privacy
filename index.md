# Privacy Policy

**Effective date:** 2026-04-26

This policy describes how the **ENCA Thermostat** mobile app (the "App")
handles your data. The App is published by **Energy Catalyst** ("we",
"us"). Contact: **<TODO: support@your-domain.example>**.

## Summary

The App is designed so that we cannot see your data. There are no user
accounts, no analytics, no advertising SDKs, and no servers operated by
us between your phone and your thermostat. Pairing happens locally by
scanning a QR code on the device.

## What we do not collect

- We do **not** ask for or collect user accounts, names, email
  addresses, or phone numbers.
- We do **not** collect location data, contacts, photos, or any other
  personal information.
- We do **not** include analytics, crash-reporting, advertising, or
  third-party tracking SDKs.

## What stays on your device

When you pair a thermostat, the App reads a QR code rendered by the
thermostat. The payload contains the thermostat's identifier and a
per-device secret key (the "API key"). Both are stored only on your
phone:

- iOS — Apple Keychain.
- Android — `EncryptedSharedPreferences` backed by the Android Keystore.

These values never leave your device except when the App uses them to
authenticate commands sent to your thermostat. Tapping **Unpair** in
the App removes them.

## What goes over the network

The App connects directly to **AWS IoT Core** to send commands to and
receive readings from your thermostat. All traffic uses TLS (MQTT over
WebSockets on port 443).

Each install acquires a short-lived AWS identity from an Amazon Cognito
unauthenticated identity pool. This identity is used solely to
authenticate the App to AWS IoT Core. It is not linked to your name,
email, or any other identifier, and is not shared with anyone other
than AWS.

AWS may observe transport-level metadata (topic names, message counts,
timestamps, source IP) in the course of operating the service. AWS's
handling of that data is governed by the AWS Privacy Notice
(<https://aws.amazon.com/privacy/>). The contents of MQTT messages are
protected by TLS in transit.

## Children

The App is rated **Everyone / 4+** and is not directed at children. We
do not knowingly collect personal information from anyone, including
children.

## Deleting your data

Because nothing is stored on our servers, deletion is local:

- **Unpair** a thermostat in the App to remove its credentials from
  your phone.
- **Uninstall** the App to remove all local data.
- **Factory-reset** the thermostat to invalidate the API key it issued
  to your phone.

There is no server-side account to delete. If you have a question
about data the App may hold, contact us at the address above.

## Security

All network traffic is encrypted with TLS. Per-device API keys are
stored using the platform's hardware-backed secure storage where
available. The App does not transmit your API keys to anyone other
than AWS IoT Core, and only as part of authenticating commands to
your own thermostat.

## Changes to this policy

If we change this policy we will update the effective date above and
publish the new version at the same URL. Material changes will be
called out in the App's release notes.

## Contact

Questions about this policy: **<TODO: support@your-domain.example>**.
