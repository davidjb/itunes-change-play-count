# Change Play Count in Music.app via AppleScript

This script works for Music.app on macOS by using AppleScript to prompt for a new
playcount to set for any songs that are currently selected in the Music.app user
interface.

This has been adapted ever so slightly from Natasha's work at
<http://www.chikaboo-designs.com/2016/01/26/applescripts-edit-your-itunes-play-count/>.

## Installation

    mkdir -p ~/Library/Music/Scripts
    cd ~/Library/Music/Scripts
    curl -L -o 'Change Play Count.scpt' https://github.com/davidjb/itunes-change-play-count/raw/master/Change%20Play%20Count.scpt

Music.app doesn't even need restarting so you can just start using the script.

Alternatively, if you want to clone this repo via Git, do that and then either
drop the script into the `~/Library/Music/Scripts` directory or hard-link it
there (Music.app doesn't support soft links).

If you make changes later (such as downloading a new version of this script),
then note that Music.app seems to cache it so ``rm`` the existing script first
and reinstall.

An [older
version](https://github.com/davidjb/itunes-change-play-count/commit/1ea469e9b6e6c84ba3316a64194173acc92a9278)
of this script works with iTunes – Apple just changed the name, thankfully.
Note that this older version is no longer maintained.

## Usage

1. Install the script.
1. Select the track(s) you wish to change playcounts for.
1. Click the script menu icon in Music and choose `Change Play Count`
1. Change the play counts to whatever you'd like them to be.  To clear a
   playcount, set to `0` or empty.

## Features

* Allows changing of playcounts in Music.app
* Prompts for input for each song
* Prompt dialog now defaults to the current playcount to avoid accidental
  clearing of counts
* Prompt dialog now shows the artist for the given song to avoid confusion

## Contributing

Pull requests with new features or bug fixes are welcome.

## License

MIT. See `LICENSE` file in this repo.
