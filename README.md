# Magic Boombox Plugin Documentation
## Installation

To integrate the Magic Boombox plugin into your project:

    Download the plugin from the Marketplace and optionally copy it to your project directory's plugin folder.

## Example Content

Example content for the Magic Boombox plugin can be found in the Examples folder of the plugin.
## Project Settings

Configure the plugin settings in your project by navigating to:
Project Settings > Plugins > Magic Boombox

These options include:

    SearchedFolder: The folder to search for music files, relative to the project's content folder, the plugin's folder, or your game's root folder.
    SearchedTypes: The type of files to search for in the folder. Defaults to .mp3 or .wav, but can be any type.

Magic Boombox is designed to automatically validate and load your music into the String Array in the actor or component. Ensure your music files are compatible with the plugin.
Usage

To get started with Magic Boombox, use the functions provided in the BP_ExampleBoombox blueprint. These functions are specifically designed to make your integration process seamless.

## Function List:
Audio Playback

    Play Random Music: Plays a random music file.
    Play Next Music: Plays the next music file in the playlist.
    Play Previous Music: Plays the previous music file in the playlist.
    Pause/Play Music: Pauses or resumes the currently playing music.
    Stop Music: Stops the currently playing music.
    Play Selected Music: Plays a specific music file.

Properties

    File Types To Find: Array of file extensions to search for.
    Sorted Music File Names: List of sorted music file names.
    Active Music Name: Name of the currently playing music file.
    Queued Music Name: Name of the music file queued for playback.

Volume Control

    Set Player Volume: Adjusts the volume of the media player component.
        Parameters:
            Transition Time: Time to fade the volume.
            Volume Level: The desired volume level.
            Fade Type: Type of fade for a smooth transition.

Additional Audio Controls

    End Play Behavior
        Behavior Setting: Choose what happens when the music file ends.
            Options:
                Play the next track in the playlist.
                Play the previous track in the playlist.
                Play a random track in the playlist.
                Stop playing music.
                Loop the current track.
                Play the specified track in QueuedMusicName.

    On End Play Reached
        Functionality: Determine what should occur when the music file reaches its end.

    Get Volume
        Functionality: Retrieve the current volume of the media player (ranging from silent to full volume).

    Get Track Progress
        Functionality: Obtain the progress of the current track as a ratio of the total track length (ranging from the beginning to the end of the track).

Enjoy the straightforward functionality of BP_ExampleBoombox for a seamless audio experience with the Magic Boombox plugin. Make sure to refer to the example content and documentation for a smooth implementation. Feel free to reach out on our Discord if you encounter any issues or have questions regarding the Magic Boombox plugin.
