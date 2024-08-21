# DOWNLOAD
Download the latest release from the releases menu on the right.
The file will be under "Assets", named something like "Blunder-3045a62.zip"

The zip is generated automatically when changes are pushed to the repository
and it will show, on the releases page, what the change that triggered a new
zip release was. The "-3045a62" part of the file name just refers to the
git commit that created the new release.


# INSTALL
1. Extract the zip and get Blunder.xml and either BlunderGui.xml OR
KaiBlunderGui.xml (NOT BOTH).
I mainly use the original GUI which is BlunderGui.xml so most improvements and
fixes will be using that but if you want to use the Kai version and you find
some issue let me know and we can do something about it.

2. Go to Package Manager on Mudlet and Install from there the two .xml files.

3. Log into Aetolia, enter the "?setup" command to initialize everything.

4. Log out and restart the client.

5. Until I change how the defup system works, the first thing you should do is
click the scripts button, go to the search field on the bottom right and
search for "defense options". From the results you get it should be the
second. Look on the right, in the editor and find any defenses in the General
table and your Class' table that you don't know yet, if any, and comment the
lines by adding -- in front of them so that the defup command won't try to
bring up defenses you do not know. (Until I redesign that system).

Example:
--def_thirdeye = "on"

This will make defup command not try to keep up the thirdeye defense.


# UPDATE
When a new version is up you have to follow this procedure in order to get a
clean update.
Log off. Open your Aetolia profile in Offline mode and:
1. Remove Blunder or BlunderGui/KaiBlunderGui depending which package is getting
 an update (or both if both are).
2. Follow the procedure from INSTALL section again.

### CAVEAT
Do to the way updates are handled (this is a Mudlet thing). Any custom
aliases/triggers/etc that you make, you should ALWAYS put OUTSIDE the Blunder
package even if they depend/use features from Blunder.
What I do is I make a "Personal" folder and save my custom stuff under there.
If you don't follow this advice, when you remove the package to update, you
will lose you custom stuff.
