# org.freecadweb.FreeCAD
This is a fork of the official freecad flatpak build repository. Its modified to build the freecad branch linkstage3 from realthunder: https://github.com/realthunder/FreeCAD
# How to build this flatpak:
* get subrepo in git (glu dependency):
  `git submodule update --init --recursive`
* add org.kde.Sdk/x86_64/5.15:
  `flatpak install org.kde.Sdk/x86_64/5.15`
* add org.kde.Platform/x86_64/5.15:
  `flatpak install org.kde.Platform/x86_64/5.15`
* add io.qt.qtwebkit.BaseApp/x86_64/5.15:
  `flatpak install io.qt.qtwebkit.BaseApp/x86_64/5.15`
* build:
  `flatpak-builder build org.freecadweb.FreeCAD.yaml`
