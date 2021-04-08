## Making a new project

This is a guide how to create a new project with your own data.

### Preparing multimedia assets

How to get your multimedia data ready to add to your AVA360VR project as assets.

#### Synched versus unsynced media files

All the synced audio and video clips to be used in a project need to be synced together so that they have the same IN and OUT points and therefore they are all of the same time duration.
This must be done outside of _AVA360VR_.
We have produced an [online video](https://youtu.be/FWZy9PK_ODw) that gives instructions how to synchronise multiple video files and export them as clips with identical IN and OUT timecodes in a non-linear video editor.

#### Synced 360 video clips

- The resolution and bit rate of the 360 video should be as high as possible, otherwise the video playback will be blocky and blurred in VR.
Use the raw footage and render at a high bit rate using the camera software (or dedicated software such as _MistikaVR_).
- The dimensions of the 360 video should be 4K or UHD, eg. from 3840x1920 up to 4096x2160.
Video at higher resolutions, eg. 8K or 6K is not supported.
- Stereoscopic 360 video is not supported in this release.
The video playback may be choppy and delayed.
- Stitch the raw footage carefully so that the stitch lines between lenses are not too visible.
- With mobile 360 cameras use stabilisation while filming or stabilise later in the camera software.
_MistikaVR_ has tools for re-stabilising, but it is not free and it takes some effort.

#### Synced audio clips

- Audio clips can be added with `WAV`, `OGG`, `MP3` format.
- Ambisonic audio is not supported in this release (but audio in AVA360VR is spatialised).

#### Unsynced audio and video clips

- Audio and video files that are not synced to the master 360 video can be added and imported.
They should be in a suitable format as above.

#### Transcripts

Transcripts should be prepared with our software DOTE (Distributed Open Transcription Environment), which is currently in beta-testing.
The transcript projects prepared with DOTE can be opened natively in AVA360VR.
Transcripts can be live edited in DOTE while viewing them in _AVA360VR_.

#### Images

Images can be imported if they are in standard formats such as `PNG`, `GIF` or `JPG`.
The size of the window displaying the image that is imported in AVA360VR is proportional to the dimensions of the image.

#### 3D models

3D models (with textures) for AVA360VR should be in `FBX` or `OBJ` format as one file.
Some models may not be importable, or if they are, then the colour textures may be missing.

### Creating a new project

It is recommended that you store all of your related projects in the same root folder, eg. `MY AVA360VR PROJECTS`.
If you do this, then you can easily jump between projects while in VR using the analysis mapping tool.

After loading _AVA360VR_, choose `Create Project`, then select the root folder where all your projects will be stored on your drive, type the project name, select the 360 video file you wish to make the master 360 (it will be copied into the new project automatically), and lastly, give a name for your first analysis.
You can have many analyses in one project, eg. each with a different combination of visible video clips, audio clips, drawings, animations, etc..
And you can have multiple versions of the same analysis, eg. indicated with the postfix `-NNN`, where `NNN` is an incremental number.

Once the project is created, you can then open any of the analysis versions you have created, reduplicate an analysis version or start a new analysis in the same project.

Each project should contain copies of all the files that available to be imported.
The files should be copied into the appropriate folder.
Some of these folders will also be where any exported files (eg. recammed 2D video clip, keyframe sequences, screenshot, comic panel generator) will be stored.

### Adding files to the new project

Every _AVA360VR_ project has the same folder structure as shown in the following diagram.

![AVA360VR folder structure](images/folders.png)

If you named your project `MY PROJECT`, then every subfolder is important and should not be renamed.
This folder structure will guide you into which folders you need to copy all the files.
When you created the project, the master 360 video was copied automatically to the correct subfolder `MY PROJECT/Video/Synced360/`.
Now you need to copy any other audio-visual files into the correct subfolders.
For example, if you have a synced audio file (eg. a wireless microphone), then copy the file into the `MY PROJECT/Audio/Synced Audio/` subfolder.

### Importing assets in AVA360VR

Once you have completed copying manually all the relevant files, then they will be available in _AVA360VR_ from the `IMPORT` menu on the left controller.
