# Change Play Count in iTunes via AppleScript

This script works for iTunes on macOS by using AppleScript to prompt for a new
playcount to set for any songs that are currently selected in the iTunes user
interface.

This has been adapted ever so slightly from Natasha's work at
<http://www.chikaboo-designs.com/2016/01/26/applescripts-edit-your-itunes-play-count/>.

## Installation

    mkdir -p ~/Library/iTunes/Scripts
    cd ~/Library/iTunes/Scripts
    curl -L -o 'Change Play Count.scpt' https://github.com/davidjb/itunes-change-play-count/raw/master/Change%20Play%20Count.scpt

iTunes doesn't even need restarting so you can just start using the script.

Alternatively, if you want to clone this repo via Git, do that and then either
drop the script into the `~/Library/iTunes/Scripts` directory or hard-link it
there (iTunes doesn't support soft links).

## Usage

1. Install the script.
1. Select the track(s) you wish to change playcounts for.
1. Click the script menu icon in iTunes and choose `Change Play Count`
1. Change the play counts to whatever you'd like them to be.  To clear a
   playcount, set to 0 or empty.

## Features

* Allows changing of playcounts in iTunes
* Prompts for input for each song
* Prompt dialog now defaults to the current playcount to avoid accidental
  clearing of counts
* Prompt dialog now shows the artist for the given song to avoid confusion

## Contributing

Pull requests with new features or bug fixes are welcome.

## License

MIT. See `LICENSE` file in this repo.
