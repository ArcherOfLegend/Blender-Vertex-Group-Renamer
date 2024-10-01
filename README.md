# Blender-Vertex-Group-Renamer
Add-on for Blender to batch rename vertex groups or bone names.
![image](https://github.com/user-attachments/assets/a9e8ff52-fcde-4a05-ac63-12818fc15e32)

# Installation:
Install .py file in Blender's add-on preferences. Should work in any version 2.8+

# Usage and Features:
Access the UI from the toolbar/sidebar (N key). It has its own tab called "Vertex Group Renamer".

## Presets
You can create, duplicate, rename, and delete presets, as well as import and export them as JSON files to share with others for projects. You can also of course edit the JSON file itself if you don't like working with the add-on's UI.
![image](https://github.com/user-attachments/assets/e9eab36d-d201-49c3-85e3-8bf11735dae7)

## Rulesets
Rulesets are where you create "rules" for your renaming. You can set certain vertex groups to be renamed something else. When you create a ruleset, you'll be given the option to assign a "prefix" to it. Read below for more info.
![image](https://github.com/user-attachments/assets/803692c2-66cc-42e3-a640-52474cf88f68)

## Prefixes
Rulesets can be given an associated "prefix" to target specific meshes and armatures that share the same prefix in their names. Most users will probably want to leave their prefixes blank unless they have a reason not to; however, it's powerful when working with multiple meshes that are linked to multiple different skeletons. You can essentially make different objects or armatures use different renaming conventions while still renaming them all in one click.

## Renaming
You can rename groups back and forth with the apply and reverse buttons. You can also sync bone renaming with vertex group renaming, so that linked armatures will also have their bones affected by the vertex group renames.
![image](https://github.com/user-attachments/assets/cf42e34f-205e-426f-94ee-42bc5d573362)

## Merging
Rules targeting the same new name will result in merged vertex groups. For example, if you make two rules, one for A to be renamed C, and another for B to be renamed C, A and B will become C and have their weights merged.

## Mirroring Names
There are mirror buttons for swapping vertex group names or armature bone names starting with 'L_' and 'R_'. Useful if for some reason the model you're working with has mirrored weights.
