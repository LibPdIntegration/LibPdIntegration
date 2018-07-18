# Patching libpd

z_libpd.patch should be applied to z_libpd.c from libpd (in libpd/libpd_wrapper). Note that this is only necessary if you want to deploy to a platform not currently supported by LibPdIntegration (at time of writing, Windows and OSX are the only supported platforms).

The patch fixes an issue where libpd doesn't allow us to reset the print hook. In other applications this might not be a problem, but due to the way Unity works (keeping native plugins loaded in the editor after the game has stopped running) it will crash the editor if you try and run the game in the editor more than once. Effectively, Unity tries to call the print hook we set when we first ran the game, which no longer exists at this point.

The patch is accurate for libpd commit a538e3e on Apr 20 2018 (the current version at time of writing). It is unlikely it will work with more recent commits.