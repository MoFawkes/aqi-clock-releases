# AQI Clock

AQI Clock is a Windows desktop clock for staff. It shows the current lesson, the time remaining, the next lesson, announcements, and timetable changes managed centrally by administrators.

> This repository contains public installer and update files only. The application source code is maintained separately.

## Download and install

1. Open the [latest AQI Clock release](https://github.com/MoFawkes/aqi-clock-releases/releases/latest).
2. Under **Assets**, download `AqiClock.App-stable-Setup.exe`.
3. Run the downloaded installer as your normal Windows user. Administrator access is not required.
4. If Windows SmartScreen appears during the pilot, select **More info**, confirm the publisher/file details, then select **Run anyway**. Code signing will be added before wider rollout.
5. Open **AQI Clock** from the Start menu if it does not open automatically.

AQI Clock supports Windows 10 version 1809 or later and Windows 11.

## Sign in

Use the email address invited by your AQI Clock administrator and the password you set when accepting the invitation. Internet access is required for the first sign-in. After a successful sync, the clock can continue displaying cached timetable information while offline.

If you have not received an invitation or cannot access your account, contact your AQI Clock administrator.

## Reset your password

Password recovery through the desktop application requires AQI Clock **v0.9.2 or later**.

1. On the sign-in screen, select **Forgot password**.
2. Enter your invited email address and request the recovery email once.
3. Open the newest recovery email on the same Windows computer.
4. Select its recovery link. Windows should open AQI Clock's **Set new password** window.
5. Enter and confirm a new password, then sign in normally.

If no email arrives, check spam and wait before trying again. Repeated requests can trigger the email provider's rate limit. Never send anyone the recovery link—it contains temporary account credentials.

## Everyday use

- **Main window:** Shows the clock, today's periods, the current lesson, countdown, and next lesson.
- **Compact mode:** Use the compact control or tray menu for a small always-on-top strip.
- **Announcements:** Select the bell to read current announcements. Opening the panel marks visible announcements as read.
- **System tray:** Closing the main window normally keeps AQI Clock running in the notification area. Use the tray menu to reopen it, sync, change display options, open Settings, sign out, or exit fully.
- **Notifications:** AQI Clock can notify you when lessons start, shortly before they end, and when announcements arrive. Windows Do Not Disturb may place notifications directly in Notification Center instead of showing a banner.
- **Settings:** Configure theme, compact mode, always-on-top, start with Windows, start minimised, close-to-tray, and notification preferences.

## Administrator features

Administrators can open **Edit timetables** to manage:

- Timetables and periods
- The Monday-to-Sunday schedule
- Date-specific overrides and closed days
- Announcements
- User roles and account activation
- Recent audited changes

Administrative editing requires an internet connection. Server permissions remain authoritative even if the desktop interface is out of date.

## Updates

AQI Clock checks this public release channel when it starts and every six hours while running. Updates download silently and are applied after AQI Clock exits; the next launch uses the new version. Your session, settings, and local timetable cache are retained across updates.

You can see the installed version and update status under **Settings → About**.

## Uninstall

Use **Settings → Apps → Installed apps → AQI Clock → Uninstall** in Windows. Uninstalling removes the application and its startup entry. Diagnostic logs may remain under `%LOCALAPPDATA%\AqiClock` so support can investigate previous problems.

## Getting help

When reporting a problem to your AQI Clock administrator, include:

- The version shown in **Settings → About**
- What you were doing when the problem occurred
- Whether Windows 10 or Windows 11 is in use
- A screenshot of the message, if it contains no password or recovery link

Never share your password, recovery link, access token, refresh token, or Supabase service-role key.