# wsb config

Scripts and configuration for Windows Sandbox.

Currently needs either Windows 10 build 18342 or later (untested),
or Windows 11.

## Installing Windows Sandbox

Not to replicate other documentation, but as quick notes.

### Installing with Powershell

As an administrator:

	Enable-WindowsOptionalFeature -Online -FeatureName "Containers-DisposableClientVM" –All

Now reboot.

### Installing with cmd.exe

As an administrator:

	Dism /online /Enable-Feature /FeatureName:"Containers-DisposableClientVM" –All

Now reboot.

## Installing the scripts and config

Copy everything in the sandbox/ directory to C:\Sandbox.

You can put them somewhere else, but you'll have to adjust the paths
within them.

## Using the scripts and config

Just locate the appropriate .wsb file in c:\Sandbox\config\ and
double-click it.

Available choices are listed below.

### sandbox/config/zoom.wsb

Downloads the Zoom installer and runs it within the Sandbox, with video
and audio passthrough enabled from the host.  This is sufficient to
allow a meeting to be joined with full audio and video.

