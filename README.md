### Optional language-specific data for Acnicoy

Additional data for Acnicoy gets uploaded as sets of assets that are part of
releases of this repository on GitHub. Note that not every release necessarily
contains all data required for a language, because files that have not changed
since the last upload might not get reuploaded again. Each release is tagged
with a version number, as well as the codes of the languages it is used for.

The repository contains information about the different release versions and the
files they contain. This information is accessed programatically by Acnicoy.
It requests the file "versions.txt" once a day to check whether the latest
release versions differ from the ones used in the program. If a change has been
detected for a language pair, it requests the corresponding version register
that is stored in a file with the name `<targetLanguage>-<sourceLanguage>.json`.

The version register maps each file to all versions available for it, including
additional information on compatibility with program versions and the filesize.
Acnicoy picks the newest file versions that are supported by the current program
version, and downloads the corresponding assets from the corresponding releases.
