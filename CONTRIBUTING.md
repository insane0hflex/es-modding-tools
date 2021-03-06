Contributing
============

To add a project to the list, just append a definition for it to the `data.json` file.

## Project Definition Format

Project definitions use the following JSON structure:

```
{
  "name": "",
  "sections": [
    ""
  ],
  "description": "",
  "homepage": "",
  "repository": ""
}
```

The `name` and `sections` keys are required, and the `sections` array must contain at least one element. The other keys can be omitted if there is no content to set their values to.

### name

The `name` key takes a string that is the project's name.

### sections

The `sections` key takes an array of strings that are used to create list section names. The project will be listed in all the sections given.

For example, if the sections for a project are `plugin parsing` and `save file parsing`, the project will be listed in the "Plugin Parsing" and "Save File Parsing" sections.

### description

The `description` key takes a string describing the project, that will be displayed below its name in the list.

### homepage

The `homepage` key takes a string that is the URL for the project's homepage, for example its website or Nexus Mods file entry.

If there is no `repository` value is set, the `homepage` URL will be used as the project's link.

### repository

The `repository` key takes a string that is the URL at which the project's source code can be found. This does not need to be a version control repository: for example, it could be where an archive containing the source code is hosted.

If the `repository` value is set, its value will be used as project's link.
