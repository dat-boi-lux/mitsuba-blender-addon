Mitsuba Blender Addon (Modified to work with Blender 2.75a/2.79b)
---------------------

Authors:
Wenzel Jakob, Francesc Juhé, Bartosz Styperek

Thank you to Jason Brenneman for modifying the code to be compatible with Blender 2.75/2.75a.

This directory contains the addon for Blender -> Mitsuba Renderer
integration. It is based on the excellent LuxBlend 2.5 code from
Luxrender project.

It also uses a custom 'extensions_framework' taken from the original
'Blender 2.5 Extensions Framework' by Doug Hammond from Blender and
with some modifications also from Luxrender project.

Mitsuba Blender exporter tries to convert all Blender scene information
to Mitsuba Renderer format. Custom properties panels are added to
Blender UI to set Mitsuba Renderer options and custom attributes.


Installation Instructions (Ubuntu 20.04):
--------------------------

Copy the 'mtsblend' folder into Blender scripts/addons directory and
then enable Mitsuba addon on 'Addons > Render' section of Blender
'User Preferences' panel.

Locate your Mitsuba installation directory. Within this directory Copy the /dist/ directory to your system: /usr/share directory. Rename the directory you just copied over to 'mitsuba'. (i.e. /usr/share/dist becomes /usr/share/mitsuba).

Navigate back to your Mitsuba installation directory. within /dist/, Copy or symlink each '.so' file within this directory to your system: /usr/lib directory.

After enabling the addon, configure the 'Path to Mitsuba Installation'
setting that appears under Mitsuba addon on the same 'User Preferences'
panel by selecting the folder: /usr/share/mitsuba (where you previously copied over mitsuba to).

Blender might have to be restarted after configuring 'Exectuable Path'
for Material preview to work.
