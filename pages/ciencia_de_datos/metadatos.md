Metadato           | Uso      | Descripción
-------------------|----------|-------------
`name`             | Paquete  | [A short url-usable (and preferably human-readable) name of the package](http://specs.frictionlessdata.io/data-package/#name)
`homepage`         | Paquete  | [A URL for the home on the web that is related to this data package](http://specs.frictionlessdata.io/data-package/#homepage)
`profile`          | Paquete  | [A string identifying the profile of this descriptor as per the profiles specification](http://specs.frictionlessdata.io/profiles/)
`comment`          | Paquete  | [Miscellaneous information about the data or methods used to produce it](http://cfconventions.org/cf-conventions/cf-conventions.html#description-of-file-contents)
`contributors`     | Paquete  | [The people or organizations who contributed to this Data Package](http://specs.frictionlessdata.io/data-package/#contributors)
`description`      | Paquete  | [A markdown formatted description of the package](http://specs.frictionlessdata.io/data-package/#description)
`history`          | Paquete  | [List of the applications that have modified the original data](http://www.unidata.ucar.edu/netcdf/docs/netcdf.html#Attribute-Conventions)
`institution`      | Paquete  | [Specifies where the original data was produced](http://cfconventions.org/cf-conventions/cf-conventions.html#description-of-file-contents)
`references`       | Paquete  | [Published or web-based references that describe the data or methods used to produce it](http://cfconventions.org/cf-conventions/cf-conventions.html#description-of-file-contents)
`sources`          | Paquete  | [The raw sources for this data package](http://specs.frictionlessdata.io/data-package/#sources)
`title`            | Paquete  | [A succinct description of what is in the dataset (written in English)](http://www.unidata.ucar.edu/netcdf/docs/netcdf.html#Attribute-Conventions)
`titulo`           | Paquete  | Traducción al español de `title`
`name`             | Recurso  | [The name is a simple name or identifier to be used for this resource](http://specs.frictionlessdata.io/data-resource/#name)
`id`               | Recurso  | Igual que [`name`](http://specs.frictionlessdata.io/data-resource/#name) pero sin ".", "-" ni "_"
`path` o `data`    | Recurso  | [Property describing the location of the data associated to the resource](http://specs.frictionlessdata.io/data-resource/#data-location)
`profile`          | Recurso  | [A string identifying the profile of this descriptor as per the profiles specification](http://specs.frictionlessdata.io/profiles/)
`description`      | Recurso  | [A description of the resource](http://specs.frictionlessdata.io/data-resource/#optional-properties)
`source`           | Recurso  | [The method of production of the original data](http://cfconventions.org/cf-conventions/cf-conventions.html#description-of-file-contents)
`title`            | Recurso  | [A succinct description of what is in the dataset (written in English)](http://www.unidata.ucar.edu/netcdf/docs/netcdf.html#Attribute-Conventions)
`titulo`           | Recurso  | Traducción al español de `title`
`name`             | Variable | [This property should correspond to the name of field/column in the data file](http://specs.frictionlessdata.io/table-schema/#name)
`axis`             | Variable | [Identifies latitude, longitude, vertical, or time axes](http://cfconventions.org/cf-conventions/cf-conventions.html#coordinate-types)
`description`      | Variable | [A description for this field](http://specs.frictionlessdata.io/table-schema/#description)
`long_name`        | Variable | [A descriptive name that indicates a variable's content (written in English). This name is not standardized ](http://cfconventions.org/cf-conventions/cf-conventions.html#long-name)
`nombre_largo`     | Variable | Traducción al espanol de `long_name`
`standard_name`    | Variable | [A standard name that references a description of a variable's content in the standard name table](http://cfconventions.org/standard-names.html)
`units`            | Variable | [Units of a variable's content](http://www.unidata.ucar.edu/software/udunits/udunits.txt)