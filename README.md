## Stock Android Privacy & Security Guide
#### Guide on how to reduce data collection on Android, while still enjoying it's security model.

This repository consolidates information on how to balance privacy and security while using a stock (or close to stock) Android version. 

This will guide you on how to neuter invasive software from Android devices, granting some level of privacy and decreasing battery consumption, while keeping the Android secuirty model intact and it's Quality-of-Life software and stability. The changes applied are not complex, and are offered within Android's and Google's Settings. I will explain my reasoning as to what changes should be applied throught the guide.

##### Intro:
Before we start, I would like to state that this guide is intended to be applied to devices that have **close-to-stock ROMs**, such as Motorola devices, but are also applicable to Google Pixel.

Why Motorola, you ask? Why, Pixels are not readly available on markets outside of the US and the EU. As such, I am making this guide thinking of those who do not have the chance to buy Pixel devices. While Motorola **is** owned by Lenovo at the time of writing, and as such likely has invasive regional practices, it also offers a ROM that is closest to stock and affordable phones worldwide with not much bloatware shipped by default.

##### Preparations:
First things first, we will do what many privacy advocates consider to be blasphemy: We will create a new Google Account. I know, I know, Google is not privacy respecting, yada, yada. We cannot, however, sacrifice security in the name of privacy, and Android's bleeding edge security features actually require your Google login to work. We are going to take advantage of those features, and of the privacy toggles available on Android.

###### Create a new Google Account:

To create your Google account, consider the following:
- Use a computer for this. Open Private Mode / Incognito Mode.
- When creating a new Google account for personal use, choose a generic name (no last name) and birthday. For gender, choose "Prefer not to say".
- When you are asked to create a new gmail address, choose "Use Existing Address", and enter a trusted email provider, such as Proton, Tuta or Mailbox for example.

Now, after you have created your account, click on the user bubble at the corner and then on "Manage your Google Account". Notice the menu at the left of your Google Account settings page. We are going to be toggleing some options there.

###### The "Data & privacy" Menu:

- Scroll down to the "History settings" section. There, enter all the listed categories (Web & App Activity, Timeline, YouTube History) and turn off each setting.
- Scroll just a bit more to the "Personalised ads" section, and open the "My Ad Center" category in a new tab. There, turn off Personalised Ads, right at the start of the webpage. Then, close the tab.
- Below "My Ad Center", open "Partner ads settings" in a new tab. There, turn off all the seetings that are available to you. Mind the "Configurations Associated to your Google Account" section.
- To the side of "Personalised Ads", open "Personal results in Search" on a new tab. Turn off "Show personal results".
- Scroll just a bit to the "Google Fit privacy" section. There, enter each section and turn off all settings. After that, close the tabs and turn your attention once more to the left side menu.

###### The "People & sharing" Menu:

- Scroll down to the "Contacts" section. Turn off all options.
- Scroll down to the "Business Features" section and turn off "Business personalization".
- To the side of "Business features", in the "Shared recommendations in ads" category, turn off "Shared endorsements in ads".

Those should be all the options at the time of writting, but browse around a bit to check if there are any more options in your country. You can add a profile picture if you'd like, on the "Personal Information" side menu (Choose one of the default options).

Do not logout or close the Google Account settings page, as we will now set up 2-Step Verification. For that, turn your attention to your Android device. Turn on your freshly formatted Android device and follow the setup prompt. Deny any permissions you are asked to grant. Connect to a secure Wi-fi and log in to your Google account. Again, remember to deny any permissions you are asked for. Finish this initial setup and turn your attention to your Google Account settings page one last time.

###### The "Security" Menu:
- Scroll down to the "How you sign in to Google" section. Enter the "2-Step Verification" category and choose "Get started". Enter your account password when prompted.
- You will be asked to enter a phone number at first. Ignore that and click "Show more options" near the end of the page. Choose "Google Prompt" and follow the instructions for the device you've just signed in.
- After that, once again go to set up 2-Step Verification. Click once again on "Show more options", but this time choose the newly added "Google Authenticator" method. Follow the instructions and add the TOTP secret to an app capable of 2FA. It is recommended to keep a copy of your Google Account password and TOTP authentication on an app that is not located on your phone at first, such as an offline KeePassXC file, and keep that on a backup hard-drive.
- Now copy your recovery codes and keep them somewhere safe. This will be your only means of recovery, in the event you can't acess any Authenticator apps.

With that, we can begin setting up the Android device on hand.

##### Setup the Android Device:

While we were setting up 2-Step Verification, Google Play Services should have downloaded all app updates / installed all the default ones for us. After that, open the app drawer and inspect the installed apps. Now open the Android Settings app.

###### Settings - Google:
Enter the Google section of the Settings app and change the following settings:
- Advertisements - Delete Advertisement ID: Yes
- Find My Device - Use Find My Device: On
- Personalize Usind Shared Data: Turn every setting off.
- Search around a bit and check the other settings, turning off anything that seems agregious.

###### Settings - System:
- Languages & input - On-screen keyboard - Gboard - Privacy: Turn every setting off.

###### Settings - Apps - See all apps:
- Google Play Services - Permissions: Turn off each one, unless there's a particular feature that needs those.
- Google Carrier Services - Permissions: Turn off each one, unless there's a particular feature that needs those.
- Google - Permissions: Turn off each one, unless there's a particular feature that needs those.

###### Settings - Battery:
- Adaptable Preferences - Adaptable Battery: On

###### Settings - Screen:
- Adaptable Brightness: On

###### Settings - Security:
- Device administrator apps - Find My Device: On
- Device administrator apps: Examine the specific features included and turn off unecessary ones.
- Trust Agents: Turn off each one, unless you know of a particular feature that needs this premission.

###### Settings - Privacy:
- Notifications on lock screen: Only show confidential content when unlocked
- Show passwords: Off
- Permission manager - Body sensors: Turn off each one, unless there's a particular feature that needs those.
- Permission manager - Physical activity: Turn off each one, unless there's a particular feature that needs those.
- Permission manager - Nearby devices: Turn off each one, unless there's a particular feature that needs those.
- Android System Intelligence - Customize the experience using your Google Account data: Off
- Personalize app data usage: Off

###### Settings - Location:
- Location Services - Wi-fi search: Off
- Location Services - Bluetooth search: Off

###### Quick Settings Menu:
- Turn off Mobile Web, Bluetooth and Location Services, turning them back on only when needed
- Edit your quick settings tiles in a way that you can easy check what settings are active at any given time, to allow better control of the data you create, for example as:
  - Wi-Fi
  - Mobile network
  - Bluetooth
  - Location
  - Do not disturb
  - Airplane mode
  - Power Savings
  - Automatic rotation
  - Flashlight

##### Optional Android Settings:
These settings give Google more data about you and how you use your device, but also can offer some much appreciated convenience. Use at your own discretion.

###### Settings - System - Backup:
You can choose which elements you back up to Google Drive, such as only backing up app data. Activating backups will opt you into backing up app and device settings automatically.
- Photos and videos: It is recommended to leave this as Off, whether or not you choose to backup app and device data.
