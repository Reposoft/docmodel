
A documentation system can be used for knowledge management.
An issue tracker can be used for knowledge management.
A knowledge management system can be modelled on issue tracking.

A documentation system has projects.
A project has documents numbered from 1 to N.
A document has a `type` property, from a system+project enum.
A document has a `status` property, from a system+project enum.
A document has a `title` property and an optional `owner`.
A project has arbitrary document property fields.
A property field has a name and a validation rule.
A document has a date-created and a date-modified.
A document contains a body.
A body consists of authoring units.
Some authoring units are meta units, imposing structure.


A document can be `cloned`.
A clone references a master.
A clone can be temporary, with no document number allocated,
or it can be persisted as a first class document.
A temporary clone can be persisted, i.e. given a document number.
A persisted clone can be cloned.

A system has `reference` types.

A document can contain a `chat`.
A chat entry has author, date and content.
A chat entry may refer to a unit in the document.
The content of a chat entry is that of a typical rich paragraph unit,
i.e. may contain references.

A documentation system can list documents based on criterias.
A document
