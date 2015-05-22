# Organogram schemas

## Background

The Prime Minister committed central government departments in May 2010 to publish items of spending from November 2010:
<https://www.gov.uk/government/news/letter-to-government-departments-on-opening-up-data>

NHS bodies now also publish their spend data in the same way.

Mandatory guidelines for releases and formats were drawn up by the HM Treasury in May 2010:
http://webarchive.nationalarchives.gov.uk/20130129110402/http://www.hm-treasury.gov.uk/psr_transparency_index.htm

This schema is based on those guidelines.

## Timeliness

"Spend is to be published one month in arrears, ie by the last working day of the month following the month to which the data relates."

## Hosting arrangements

"All data must be published and listed on the data.gov.uk index. The metadata descriptions will need to be maintained for all of the published data. Each department will need to create and maintain their metadata entry. ... Departments may choose to post data on behalf of entities
in their family, either separately or as part of a consolidated return. If there are no
transactions in a given month, a nil return should be submitted."

"The files are to be uploaded in CSV file format. ...  The CSV file must have precisely one header line with field names exactly as in the example file supplied. Values must be separated by a comma character, with a new line between separating transactions. Text values that contain a comma must have a `"` character at the start and end of the value. This format is the behaviour of Excel when using the "Save As" function selecting CSV as the file type" NB That you should ensure the date column shows in DD/MM/YYYY format before you do the "Save As", to ensure it is saved that way.
