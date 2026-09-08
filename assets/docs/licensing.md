# TalkNClip licensing

## License model

TalkNClip uses Freemius for purchases and license management. A one-time purchase includes a lifetime license for the purchased version, with no subscription and up to two device activations. This does not promise free upgrades to every future major version.

## Activation

An internet connection is required for initial activation and periodic license validation. If you already have a key:

1. Open **Settings → License**.
2. Paste your key into **License key**.
3. Select **Activate**.

TalkNClip activates and validates the license before enabling licensed actions. A restart should not normally be required. Do not publish or share your license key.

## Device limit

A license supports up to two activated devices. If both activation slots are in use, activation on a third device will be rejected. Deactivate another installation before activating the new computer.

## Moving to another computer

On the old computer, open **Settings → License → Deactivate this computer** while connected to the internet. Wait for confirmation before removing the application, when possible.

You can then use the same license key to activate TalkNClip on another computer, within the two-device limit. If you no longer have access to the old computer, see the [support guide](support.md) for private license assistance.

## Offline use

Initial activation requires internet access, and TalkNClip periodically connects to validate the license. After successful validation, locally cached license information allows continued use for a limited offline grace period.

A network failure does not immediately invalidate a recently validated license. If license verification is required after the offline grace period, connect to the internet and select **Settings → License → Check license**.

Voice recognition remains local/offline after the selected voice model is installed. Freemius licensing communication is separate from microphone capture and voice recognition; microphone audio is not sent to Freemius.

## Deactivation

**Deactivate this computer** releases one activation slot after the license service confirms deactivation. It requires a connection to that service.

Uninstalling TalkNClip or deleting local application data alone does not release the activation slot. Deactivate from **Settings → License** first, when possible.

## License provider

Freemius handles TalkNClip checkout and license management. The application exchanges the licensing information needed for activation, validation, and deactivation with Freemius.

Payment and card details are not entered or stored inside TalkNClip. The application does not need your name or email address for normal local license validation. Sensitive license data is protected locally using Windows user-specific protection.

## Get a license

1. Open **Settings → License**.
2. Click **Buy TalkNClip**.
3. The Freemius checkout opens in your default browser.
4. Complete the purchase.
5. Copy the license key received after purchase.
6. Return to TalkNClip and paste it into **License key**.
7. Click **Activate**.

Opening or closing checkout does not activate or change your license. Payment is completed in the browser, outside TalkNClip.

For purchase, license, or account-specific support, contact [talknclip.support@gmail.com](mailto:talknclip.support@gmail.com). Never post your license key in a public GitHub issue.

## Privacy

See [Privacy and local data](privacy.md).
