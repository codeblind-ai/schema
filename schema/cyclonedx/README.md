# CycloneDX Schemas

`flashlight` generates a CycloneDX Bom output. We want to be able to validate the CycloneDX schemas
(and dependent schemas) against generated flashlight output. The best way to do this is with `xmllint`,
however, this tool does not know how to deal with references from HTTP, only the local filesystem.
For this reason we've included a copy of all schemas needed to validate `flashlight` output, modified
to reference local copies of dependent schemas.

You can get the latest schemas from the [CycloneDX specifications repo](https://github.com/CycloneDX/specification/tree/master/schema).
