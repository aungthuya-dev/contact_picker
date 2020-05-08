# ContactPicker plugin for Flutter

[![pub package](https://img.shields.io/pub/v/contact_picker.svg)](https://pub.dartlang.org/packages/contact_picker)

With this plugin a Flutter app can ask its user to select a contact from his/her address book. The information associated with the contact is returned to the app.

This plugin uses the operating system's native UI for selecting contacts and does not require any special permissions from the user.

Currently, the plugin only supports picking phone numbers. However, it should be easy to extend the plugin to request other properties from a contact (e.g. addresses) or to obtain the entire record of a contact (PRs are welcome).

## Using the plugin

Follow the instructions in the [Installing](https://pub.dartlang.org/packages/contact_picker#pub-pkg-tab-installing) tab on pub.

After that, instantiate `ContactPicker` in your Flutter app and call `selectContact` on it to bring up the UI for selecting a contact. The function returns with the selected `Contact` object once the user has made a choice (or `null` if the user didn't select anything).

See `example/lib/main.dart` for an actual usage example.

=======================================================================

# Using this Frok Directly (branch : v1.0.0)

This is a fork of https://github.com/goderbauer/contact_picker repository.
There was an issue while building APK for android OS.

There are a lot of plugins for this kind of functionality.
I checked all and found some kind of issues and all are a little outdated.

So, I forked this repository and Fixed the issues.
I also reimplemented and cleaned the codes by by using latest sdks and plugin version by avoiding deprecated methods and classes.
I created pull request to merge and update original plugin.
But the developer is not active for a while and we can't know when he merge my pull request.

I don't also want to create and publish new plugins to https://pub.dev.

If you meet some problems with other plugins and want to try my fixes, you can add this repository directely as dependency.

    dependencies:
      contact_picker:
        git:
          url: https://github.com/aungthuya-dev/contact_picker.git
          ref: v1.0.0
      
There is also an example project inside `/example` folder.
