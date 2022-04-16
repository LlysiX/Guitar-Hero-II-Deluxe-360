# Guitar-Hero-II-Deluxe-360
This Repo contains everything you need to build an ark for gh2dx 360, and also run the included xex on PC with an included build of Xenia.
Xenia is pre setup for portable instalation with it's own config file that disables vsync, and sets an option in this specific build (max_queued_frames = 3)
You can install song packs directly in your local copy of this repo in
>\content\415607E7\00000002\XXXXXX
Where XXXXXX is the name of your song pack, containing both a "songs" and a "config" folder.
con/live files are not supported.
You can find Vanilla song packs for [GHIIDX](https://drive.google.com/file/d/1xwX_Dv17WDFldZ0mDWZu71FLUI-CTywx/view?usp=sharing) and [GH80SDX](https://drive.google.com/file/d/1KJxH51N2yQdQXlNA9MmyrI1bGfdB6Hxz/view?usp=sharing) here.
Pad play is not currently available in this build.
Instead we have opted to treat all connected controllers as a guitar.
This can allow more controller compatibility, but also allow online coop via parsec. We tried it, it's really fun.

## Install
Setting up GHIIDX 360 for the first time is meant to be as easy as possible.
As well, it is designed to allow you to automatically recieve updates as the repo is updated.
Simply run "_init_repo.bat".
This will walk you through installing a couple dependencies, [Git for Windows](https://gitforwindows.org/), and [Dot Net 6.0 Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/6.0/runtime).
git is required for you to take advantage of auto updating via github pulls.
dot net is required to build an ARK file, the archive format the game needs to run.
You can setup git with all default options, same with dot net.
Once the dependencies are installed, git will pull the repo and make sure you are completely up to date.
Once all has completed simply run "_gh2.bat"
This script will pull the repo again for updates, build the ARK for you, and finally, launch the game in Xenia. All in one script.
A specific build of x360ce_x64 that supports guitar mappings is also included if you need it.
It is recommended to always run the game with gh2.bat to ensure everything is up to date, as currently this project is highly WIP