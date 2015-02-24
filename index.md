
A documentation system can be used for knowledge management.
An issue tracker can be used for knowledge management.
A knowledge management system can be modelled on issue tracking.

A documentation system has projects.
A project has documents numbered from 1 to N.
A document has a `type` property, from a project enum.
A document has a `status` property, from a project enum.
A document has a `title` property and an optional `owner`.
A project has arbitrary document property fields.
A property field has a name and a validation rule.
A document has a date-created and a date-modified.
A document contains a body.
A body consists of authoring units.
Some authoring units are meta units, imposing structure.

A unit may contain `reference`s.

A document can be `clone`d.
A clone references a master.
A clone can be `temporary` or it can be assigned a document number.
A non-temporary clone can be cloned.

A document can contain a `chat`.
A chat entry has author, date and content.
A chat entry may refer to a unit in the document.
The content of a chat entry is that of a typical rich paragraph unit and as such may contain references.

A body and/or property modification is always a chat entry.
Incoming references are chat entries.
The project `timeline` consists of all chat entries in chronological order.

A documentation system can list documents based on property criterias.
A list must follow Access Control rules of the system.

A documentation system might extract snippets of referenced content and display as read-only content.

A document can have 0+ `attachment`s.

A project can have a `media archive`.
