# Trilingual input method shortcuts

## About
This repo contains a script to switch in between trilingual inputs. The script can be used conveniently by inporting it in [karabiner](https://karabiner-elements.pqrs.org/).

## What it does

As is documented in the `script.txt` file, this allows `Right_Option+1` to switch to the English input method, `Right_Option+2` to switch to Chinese, and `Right_Option+3` to Japanese.

## How to use

1. When Karabiner is running, go to `Preferences`;
2. Go to `Complex modifications` tab;
3. On the bottom-left corner, click `(+) Add rule`;
4. On the top of the new window that opened, click `(cloud) Import more rules from the Internet (open a web browser)`;
5. Go to any script, click on the arrow to the right of the blue `Import` button, and find `Edit JSON (Open external site)`; (There's gotta be a better way to do this, but this is at least working)
6. In the new page that opened, find a text box with `Paste existing modification here to edit`, paste the content of `script.txt` in this GitHub repo in that text box;
7. Click `Install!` and follow the new pop-ups in Karabiner to enable the shortcuts. 

## How to tweak

#### Input methods of other languages or third-party input methods

Click the Karabiner icon and click `Launch EventViewer`. In the `Variables` tab in EventViewer, the current `"input_source"` variable gives the relevant ids for the current input method. Simply replace the current parameters under the `"select_input_source"` variable in `script.txt` to let Karabiner know what input method variables to switch to. 
