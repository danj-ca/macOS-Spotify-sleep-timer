# Spotify sleep timer for macOS

AppleScript service to pause Spotify and put your Mac to sleep. From script found here: https://www.reddit.com/r/mac/comments/1dw6og/i_made_a_sleep_timer_for_spotify_for_those_of_you/, with a tweak:

(The script as given on Reddit subtracts `the player position` from `duration of the current track` so that Spotify doesn't pause until the current track finishes. In my experience (with version `1.0.86.337.ga8d5cef9` of the Spotify app), `duration of the current track` is a value in *milliseconds* while `the player position` is a value in seconds. I had to divide the duration by 1000 to achieve the expected results.)

## Dependencies

The [Spotify app for macOS](https://www.spotify.com/download/mac/) needs to be installed.

## Installation

A Workflow Service is a Package—if you download the `Set Spotify sleep timer.workflow.zip` file and open the `.workflow`, macOS will ask you if you want to install the service. You can alternatively open it in Automator to view its contents.
