---
title: Energy Catalyst Connect — Privacy Policy
---

# Privacy Policy

**Effective date:** [TO CONFIRM: effective date]

This policy describes how the **Energy Catalyst Connect** app handles
your information. "The app" means the Android app
(`com.energycatalysttech.hpclient`), the iPhone and iPad app (when it
is released), and the web app at
**connect.energycatalysttech.net**. The app is published by
**Energy Catalyst** [TO CONFIRM: legal entity name, e.g. "Energy
Catalyst Technologies LLC"] ("we", "us"). Contact:
**support@energycatalysttech.com**.

The app is offered in the United States only.

## Summary

- You need an account to use the app. We keep your email address and,
  if you add them, your name, phone number and company.
- Your heat pump, not your phone, sends its operating data (such as
  temperatures, energy use and alarms) to our servers. The app shows
  you that data for the homes your account is linked to.
- Your account can view your system. It cannot change your heat pump's
  settings.
- There is no advertising, analytics, crash-reporting or tracking
  software in the app. We do not sell your information.
- Our servers are in the United States (Amazon Web Services, Ohio
  region).
- You can ask us for a copy of your information, or to delete your
  account, at **support@energycatalysttech.com**.

## Information we collect

### Your account

- **Email address.** This is how you sign in. If your installer or
  Energy Catalyst invites you, we use it to send the invitation.
- **Password.** If you sign in with a password, it is handled by our
  sign-in service, Amazon Cognito. The password itself is never sent
  to us or stored by us.
- **Google or Apple sign-in.** If you choose "Continue with Google" or
  "Continue with Apple", we receive only your email address and
  whether it is verified. We do not receive your name, photo or
  contacts. Apple may give us a private relay address instead of your
  real one. If an account with the same email already exists, the two
  are linked so you keep one account.
- **Profile details you choose to add** in Settings: a display name,
  phone number and company.
- **Your account type** (homeowner, installer/contractor or Energy
  Catalyst administrator) and **which homes** your account can see.
- **Your acceptance of these documents:** which version of the Terms of
  Service and this Privacy Policy you accepted, and when.
- **Alert preferences:** whether you want email alerts (on by default)
  and SMS alerts (off by default) about faults and status changes.
  [TO CONFIRM: our servers store this choice, but no email or SMS
  alerts are sent yet. Before publishing, either (a) keep this
  sentence: "We store your choice. Alerts are not sent yet; we will
  update this policy, and name the service that sends them, before
  they start," or (b) launch alerts first and name the email/SMS
  provider in "Who we share information with".]
- **API tokens**, if you create one (Über Geek mode, API page): the
  name you give it, its first 12 characters, and when it was created,
  expires and was last used. The token itself is stored only as a
  one-way fingerprint (hash), so we cannot read it back.

### Your home and your heat pump

- **Pairing.** To link your account to a heat pump, you scan or type
  the short-lived code shown on the heat pump's own screen (a code is
  valid for about 10 minutes). Our server checks the code and adds
  your account to that home. On the phone apps the camera is used only
  to read this code (the web app has no scanner; you type the code).
  The image is processed on your device and is not saved or sent to
  us. On Android, the scanner uses Google Play services' on-device
  barcode reader (ML Kit).
  [TO CONFIRM: Google states that ML Kit may send Google usage and
  performance metrics (not the camera images). Decide whether to say
  so here.]
- **Home address.** The address of the home where the system is
  installed. It is entered on the heat pump's screen (by you or your
  installer) and sent to us by the heat pump's controller.
- **Operating data from your equipment.** Your heat pump, hot water
  tank, controller and thermostats send readings over their own
  internet connection, for example: temperatures, humidity, target
  temperatures, operating modes, power and energy use, alarms and
  faults, equipment identifiers and software versions, and the names
  given to zones and thermostats. This data is stored against your
  home, and anyone whose account is linked to that home can see it
  (see "Who can see your information").

### Technical information

- **Server logs.** When the app talks to our servers, we record
  technical details of each request, such as your IP address, the
  time and what was requested. We use them to keep the service
  working and secure.
- We do **not** collect your device's location, contacts, photos or
  advertising identifier.
- The app contains **no** third-party analytics, crash-reporting,
  advertising or tracking software.
- **Web app only:** your browser loads the app's graphics engine
  (Flutter's CanvasKit) and, for characters the app's own fonts lack,
  fallback fonts from Google's servers (`www.gstatic.com` and
  `fonts.gstatic.com`). Google receives your IP address with these
  requests, as with any website that loads files from it. The phone
  apps have their fonts built in.

### Information that stays on your device

- **Display preferences**, such as units, language, dark mode, the
  energy prices you enter for savings estimates, which heat pump to
  show, and which weather station to use. They are kept on your device
  for your account and are not sent to us.
- **A cache of recent readings**, so the app loads faster. It is
  deleted when you sign out.
- **Your sign-in session**, until you sign out.
- **Your own weather station (phone app only).** If you link a
  Weather Underground personal weather station, its API key and
  station ID are kept in your phone's secure storage (Android Keystore
  or Apple Keychain). The phone sends them only to Weather Underground
  (The Weather Company) to fetch the station's readings. They are
  never sent to us. Signing out does not remove them; unlinking the
  station in Settings does. (Uninstalling also removes them on
  Android. On iPhone and iPad, iOS can keep secure-storage items after
  an app is deleted, so unlink the station first.)
  [TO CONFIRM: we plan to move this setting to our servers, per home
  and encrypted. When that ships, replace this paragraph with: "If you
  link a Weather Underground personal weather station to your home, we
  store its station ID and your API key on our servers. The key is
  encrypted, only its last four characters are shown back in the app,
  and our servers use it only to fetch that station's readings from
  Weather Underground. Every account linked to the home sees the
  station's readings. Removing the station deletes the key."]

## How we use information

- To show you your system's live status and history, and estimates
  such as efficiency, running cost, savings and CO₂ avoided.
- To show local weather. Our servers use your home address to find the
  nearest public weather stations and fetch outdoor temperatures and
  forecasts. Your ZIP code is used to look up your regional power
  grid's CO₂ intensity (from the U.S. EPA's eGRID data, which we keep
  on our own servers).
- To tell you whether your home is among the most efficient homes we
  monitor. You see only your own home's standing, never another
  home's data.
- To send account emails such as invitations, verification codes and
  password resets. Amazon Cognito sends these for us.
- So your installer and Energy Catalyst can monitor, diagnose and
  maintain your system.
- [TO CONFIRM: "To improve our heat pumps and the app, for example by
  studying how systems perform across many homes." Keep this only if
  it is how you use the data.]
- To keep the service secure, prevent misuse and meet legal
  obligations.

## Who can see your information

- **People linked to your home.** Anyone who pairs with the code on
  your heat pump's screen, or whom we or your installer add, can see
  your home's data in the app. Contact us to remove someone.
- **Your installer or contractor**, if your home is assigned to them.
- **Energy Catalyst staff.** Our administrators can see all homes, and
  the list of accounts with their email, name, phone number and
  company. They can invite and disable accounts, and change heat pump
  settings remotely to support your system.

## Who we share information with

We do not sell your personal information or share it for targeted
advertising. We share it only as follows.

**Service providers** that run the service for us:

- **Amazon Web Services (AWS):** hosting, databases, sign-in (Amazon
  Cognito), the connection to your heat pump (AWS IoT Core) and
  account emails. AWS's handling of data is governed by the AWS
  Privacy Notice (<https://aws.amazon.com/privacy/>).
- **Google and Apple**, only if you choose to sign in with them. They
  learn that you signed in to the app.
- **Google (web app only)**, which serves the graphics engine and
  fallback fonts described under "Technical information".
- **Internal engineering tools.** Our engineers use dashboards
  (Grafana, run on our own AWS account) and a chat assistant in Slack
  that answers their questions about system data with the help of an
  AI provider. These tools work with equipment data and home
  identifiers.
  [TO CONFIRM: whether to name Slack and the AI provider (enca-iac
  configures Anthropic), what data the assistant can reach (equipment
  data; may include the home address the controller reports), and
  that the provider's terms do not let it train on or keep our data.]

**Public data services** our servers or your phone ask on your behalf:

- **U.S. Census Bureau geocoder** and, if it finds no match,
  **OpenStreetMap Nominatim**: our servers send your home's street
  address (Census) or city, state and ZIP code (Nominatim), never your
  name or contact details, to get map coordinates.
- **NOAA (National Weather Service and National Centers for
  Environmental Information):** our servers send those coordinates to
  find nearby weather stations, forecasts and temperature history.
- **Weather Underground (The Weather Company)**, only if you link your
  own weather station (see above).
- **Update checks.** On Android, the app asks Google Play whether a
  newer version is available. On iPhone and iPad, it asks Apple's App
  Store for the app's latest version. On the web, it checks a version
  file on our own site. These checks send nothing about you.

**Legal and business reasons:** when the law requires it, to protect
the rights and safety of our users, Energy Catalyst or others, or as
part of a merger, acquisition or sale of our business, in which case
this policy continues to apply.
[TO CONFIRM: wording of this clause.]

## Where information is stored

Our servers and the information we store are in the United States, in
AWS's US East (Ohio) region. The web app is delivered through AWS's
worldwide content delivery network (Amazon CloudFront).

## How long we keep information

- **Account and profile:** while your account exists. When you ask us
  to delete your account, we delete your sign-in account, profile,
  home links and API tokens. Database backups may keep a copy for up
  to 35 days.
  [TO CONFIRM: backup window. Our databases use AWS point-in-time
  recovery; 35 days is AWS's default and is not set explicitly in our
  configuration.]
- **API tokens:** until you revoke them; deleted automatically 30 days
  after they expire.
- **Equipment operating data:** detailed readings and one-minute
  summaries for 1 year, ten-minute summaries for 3 years, and hourly
  summaries for as long as we operate the service. This data belongs
  to the home and its equipment, not to one account, so it is not
  deleted when one account is deleted.
  [TO CONFIRM: what happens to a home's data when the owner asks, or
  when the home is sold, e.g. "On request from the homeowner we will
  delete or de-identify the home's data."]
- **Server logs:** 14 days for app requests and 7 days for equipment
  connection logs.
  [TO CONFIRM: whether load balancer access logs are switched on in
  production and how long they are kept.]

## Security

- All traffic between the app and our servers is encrypted (HTTPS,
  TLS 1.2 or newer). Your heat pump connects to AWS IoT Core over an
  encrypted connection with a device certificate.
- Our servers check, on every request, which homes your account is
  linked to, and return data only for those homes. API tokens can only
  read data and never have administrator rights.
- Information in our databases is encrypted at rest by AWS.
- No method of transmission or storage is completely secure, but we
  work to protect your information.

## Your choices and rights

- **See and change** your name, phone number and company, and your
  alert preferences, in the app's Settings.
- **Download your home's history** as a spreadsheet (CSV) from Über
  Geek mode.
- **Ask for a copy, a correction, or deletion** of your information or
  your account: email **support@energycatalysttech.com** from the
  address you sign in with, so we can confirm it is you. We will reply
  within [TO CONFIRM: response time, e.g. 30 days]. Your heat pump
  keeps working without the app.
- **Sign out** to remove the cached readings from your device;
  **uninstall** the app to remove what it keeps on your device (see
  the note on iPhone secure storage above).
- Depending on the state you live in, you may have further rights over
  your personal information. Contact us to use them. We will not treat
  you differently for doing so.
  [TO CONFIRM: whether state privacy laws such as California's
  (CCPA/CPRA) apply to Energy Catalyst, and whether a state-specific
  section is needed.]

## Children

The app is not directed to children under 13, and we do not knowingly
collect personal information from them. Accounts are for adults
[TO CONFIRM: minimum age, e.g. 18, to match the Terms of Service].
If you believe a child has given us personal information, contact us
and we will delete it.

## Changes to this policy

If we change this policy we will update the effective date above and
publish the new version at the same address. If we make significant
changes, the app will ask you to review and accept the policy again
the next time you sign in.

## Contact

Questions about this policy or your information:
**support@energycatalysttech.com**.

[TO CONFIRM: postal address of Energy Catalyst.]
