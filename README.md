# Calendar Import/Export

This app allows you to import/export your calenders using ics files without using Google synchronization services.

For more information, see http://sufficientlysecure.org/android/.

| [Google Play](https://play.google.com/store/apps/details?id=org.sufficientlysecure.ical) | [F-Droid](https://f-droid.org/app/org.sufficientlysecure.ical) |

# Build

## Prerequisites

1. Run the _Android SDK Manager_ (shell command: ``android``)
2. Expand the "Extras" directory and install "Android Support Repository",
   "Android Support Library" and "Google Repository".
3. Make sure the *ANDROID_HOME* environment variable is set and points to your Android SDK
   install directory (shell command ``export ANDROID_HOME=~/AndroidSDK/``)
4. Make sure the Android SDK directories "platform-tools", and "tools" are in your
   *PATH* (shell command ``export PATH="$ANDROID_HOME/platform-tools/:$ANDROID_HOME/tools/:$PATH``)

## Build with Gradle

1. Run the Gradle wrapper (shell commands ``./gradlew build``, ``./gradlew clean`` etc)
2. Run ``./gradlew --help`` for help and ``./gradlew tasks`` for a list of available build tasks
3. If needed, edit "CalendarImportExport/build.gradle" to change the "compileSdkVersion"
   and/or "buildToolsVersion" numbers to match what you installed using the SDK Manager
4. If needed, edit "CalendarImportExport/build.gradle" to change the "com.android.support:support-v4"
   version number to match the version of "Android Support Library" you installed
   using the SDK Manager

## Build with Android Studio

1. Start Android Studio
2. Choose the "Import project" option.
3. Select the "build.gradle" file in this directory and click OK.
4. Once imported, use the build action from the "Build" menu.

# Contribute

Fork the git repository, make changes and submit a pull request with the details.

## Bugs

Bugs can be raised at [Github](https://github.com/SufficientlySecure/calendar-import-export/issues).

## Translations

Translations can be submitted at [Transifex](https://www.transifex.com/sufficientlysecure/calendar-import-export/).

# Coding Style

## Code
* Indentation: 4 spaces, no tabs
* Maximum line width for code and comments: 100
* Opening braces don't go on their own line
* Field names: Non-public, non-static fields start with m.
* Acronyms are words: Treat acronyms as words in names, yielding !XmlHttpRequest, getUrl(), etc.

See http://source.android.com/source/code-style.html

## XML
* XML Maximum line width 999
* XML: Split multiple attributes each on a new line
* XML: Indent using spaces with Indention size 4

See http://www.androidpolice.com/2009/11/04/auto-formatting-android-xml-files-with-eclipse/

# Licenses
Calendar Import/Export is licensed under the GPL v3+.
The file LICENSE includes the full license text.

## Details
Calendar Import/Export is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

Calendar Import/Export is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with Calendar Import/Export.  If not, see <http://www.gnu.org/licenses/>.

## Libraries

* iCal4J  
  https://github.com/ical4j  
  See LICENSE.iCal4j

* Apache Commons  
  http://commons.apache.org  
  Apache License v2

* backport-util-concurrent  
  http://backport-jsr166.sourceforge.net  
  Public Domain

## Images

* icon.svg  
  Based on Tango Icon Library and RRZE Icon Set  
  http://tango.freedesktop.org  
  http://rrze-icon-set.berlios.de  
  Public Domain (Tango Icon Library) and Creative Commons Attribution Share-Alike license 3.0. (RRZE Icon Set)
