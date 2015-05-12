# Organogram schemas

## Background

The Prime Minister committed central government and agencies to publish organograms of all staff positions, including data on senior staff names, grades, job titles & salaries from October 2010:
<https://www.gov.uk/government/news/letter-to-government-departments-on-opening-up-data>

NB Local authorities publish their senior staff data in a different format - see the LGA guidance: <http://schemas.opendata.esd.org.uk/OrganisationStructure>

## Data collection and publication

The data is collected twice a year - snapshots of the roles on 31st March and 30th September, to be published on data.gov.uk by 6th June and 6th December respectively.

At the time of writing the organograms are published at <http://data.gov.uk/organogram/>. The web interfaces includes a drop-down to select different organizations, a "Version" slider to select releases for the data at previous time snapshots and a "Sources" button for links to the Linked Data API, which is a web interface offering navigation through and chunks of the data in RDF serializations.

The Cabinet Office provides departments with XLS template file, which is completed with the data and is then submitted into the data.gov.uk Organogram Tool. This system performs validation, rounds salaries to the nearest 5k and puts the data into RDF format. The RDF is put into the organogram triple store (for SPARQL queries) and served in the Linked Data API.

In the near future, the RDF and CSV data will be provided for download in dataset records in data.gov.uk automatically. So far, several organizations have provided their own copies of the organogram data in CSV format on data.gov.uk and gov.uk manually.

## Schemas

The organogram data comes as two CSV files - one for Senior Staff and a less detailed one for Junior Staff. All roles have an ID and all roles apart from the head of the organization reference its 'parent' role ID, allowing the drawing of the tree chart / org chart.

Schema files are provided for the CSV files:

organogram-senior-staff-csv-schema.json
organogram-junior-staff-csv-schema.json

These provide basic information about the table structure in the CSV, in JSON Data Schema format. Users can use these schemas to run basic validation checks on the CSV files using these services:

* [csvlint.io](http://csvlint.io/)
* [Good Tables](http://okfnlabs.org/projects/goodtables/)

