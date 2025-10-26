
# Live Earth Wallpapers Shortcut

  

These files combined with Automations located inside the native Shortcuts app allows the device to automatically change the Wallpaper based on the user initial selection of source.

  

The idea for this project comes from Marcus Mendes, Guilherme Rambo, and CocaTech, inspired by DownlinkApp, and it uses the same sources they shared on [sources page](https://downlinkapp.com/sources.json).

  

## Project Structure

To keep it easy to maintain, the project uses two Shortcuts

  

### Live Earth Settings

- Creates a file called `settings.json` on `iCloud Drive/Shortcuts/Data/Earth Live Wallpapers` folder

- Shows a list of source options where user needs to pick one

- Saves the selected option into `settings.json` file

- If the user runs this shortcut again, the content of `settings.json` is replaced by the new selected source

  

[Direct download of the latest version of Live Earth Settings](https://github.com/deblynprado/live-earth-wallpapers/raw/refs/heads/main/Live%20Earth%20Settings.shortcut)

  

### Live Earth Wallpapers

- Read the `settings.json` file

- Download the Wallpaper image based on the location found on `settings.json`

- Apply the download image as a Wallpaper on the device

[Direct download of the latest version of Live Earth Wallpapers](https://github.com/deblynprado/live-earth-wallpapers/raw/refs/heads/main/Live%20Earth%20Wallpapers.shortcut)

## Alternative Downloads
If the direct link to .shortcut files is not working, you can [download the .zip](https://github.com/deblynprado/live-earth-wallpapers/archive/refs/heads/main.zip) version of this repository and get both shortcuts from there.

  

## How to Use

- Download Live Earth Settings Shortcut

- Import Live Earth Settings into your Shortcuts App

- Tap on the shortcut to run

  - System will prompt a list of options, choose one

  

- Download Live Earth Wallpapers Shortcut

- Import Live Earth Wallpapers into your Shortcuts App

- Every time you want to "reload" the wallpaper just run this Shortcut again

  

## Automation

Shortcuts App doesn't allow shortcuts to run without a _trigger_. The solution to automatically refresh your selected Wallpaper is using the Automations option inside the Shortcuts App.

**Visual Guide:** Watch the [Automation Setup Video](Automation%20Setup.MP4) for a step-by-step visual tutorial.

  

### Step-by-Step Instructions:

- Open Shortcuts App

- Open the "Automation" tab

- On right-top, use the "+" or "New Automation" button to create a new automation

- Use the following setup:

  - *Click/Tap:* Time of the Day

  - *Click/Tap:* Time of Day

  - Set up the Hour and Minute when you want the Wallpaper to be updated

  - *Repeat:* Daily

  - *Select:* Run Immediately

  - *Disable:* Notify When Run

  - *Click/Tap*: "Next" at top-right

  - Choose the *Live Earth Wallpapers* shortcut

  

That's all! This automation will run on the hour-minute you set up and will refresh your wallpaper downloading the new version of the same source you selected before.

You can repeat this automation as many times as you want