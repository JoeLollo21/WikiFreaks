# WikiFreaks Metadata Application Profile:
WikiFreaks' metadata profile defines the type of metadata that collected by the repository, and its encoding and authority control.
<br><br>
The structure of this profile was inspired by that of the [Qualitative Data Repository](https://qdr.syr.edu/content/qdr-metadata-application-profile) from Syracuse University. 
## Metadata Schema:
The WikiFreaks repository uses a unique, in-house metadata schema combining three standards. It most closely maps to the <a href="https://datacite.org/">DataCite</a> schema, which is widely used in the documentation of research data and easily facilitates end-users' access to data.
<br><br>
Information on data licensing and edits made to the data comes from the <a href="https://ddialliance.org/">DDI (Data Documentation Initiative)</a> schema, as this content is not present in the DataCte schema yet is integral to the repository's value of accountability for the open uploading and reuse of data.
<br><br>
Lastly, temporal elements – namely for the creation and modification of data and the temporal coverage of datasets – come from the <a href="https://www.dublincore.org/">Dublin Core Metadata Initiative (DCMI)</a> schema.
<br><br>
Below you will see all metadata elements in use, including potential vocabulary or standard restrictions and notes on usage. Fields are listed in order of appearance in the WikiFreaks catalog. 

## Metadata Elements:
<table>
	<tr>
		<th>Element</th>
		<th>Common<br>Name</th>
		<th>Namespace</th>
		<th>Status</th>
		<th>Encoding</th>
		<th>Definition and Rules</th>
	</tr>
	<tr>
		<td><strong>&lt;dci:creator&gt;</strong></td>
		<td>Creator</td>
		<td>DataCite</td>
		<td>Mandatory</td>
		<td>String</td>
		<td>	The individual(s) involved in creating the data, or the authors of a publication where the data is used.
			<br><br>To credit multiple creators, repeat this element.
			<br><br><strong>Name Format:</strong> Last Name, First Name
		</td>
	</tr>
	<tr>
		<td><strong>&lt;dci:nameIdentifier&gt;</strong></td>
		<td>Creator's Name Identifier</td>
		<td>DataCite</td>
		<td>Optional</td>
		<td>String</td>
		<td>	A unique identifier to verify the creator.
			<br><br>The source, such as the creator's <a href="https://orcid.org/">ORCID ID</a>, must be specified within the element tag.
		</td>
	</tr>
	<tr>
		<td><strong>&lt;dci:affiliation&gt;</strong></td>
		<td>Creator's Affiliation</td>
		<td>DataCite</td>
		<td>Mandatory</td>
		<td>String</td>
		<td>	The full name of the creators' organizational or institutional affiliation.
		<br><br>For submitters without an academic or professional affiliation, use "<strong>Independent</strong>."
		</td>
	</tr>
	<tr>
		<td><strong>&lt;ddi:dataProcessing&gt;</strong></td>
		<td>Data Processing Done</td>
		<td>DDI</td>
		<td>Mandatory</td>
		<td>String</td>
		<td>Any free-text information that uploaders and/or creators are willing to provide surrounding the dataset, such as the areas of Wikipedia it covers.</td>
	</tr>
	<tr>
		<td><strong>&lt;dci:PublicationYear&gt;</strong></td>
		<td>Publication Year</td>
		<td>DataCite</td>
		<td>Mandatory</td>
		<td>Integer</td>
		<td>	The year when the data was made publicly available on the WikiFreaks repository. 
		<br><br>Must be a four-digit number representing a year.
		</td>
	</tr>
	<tr>
		<td><strong>&lt;dcterms:created&gt;</strong></td>
		<td>Date Created</td>
		<td>Dublin Core</td>
		<td>Mandatory</td>
		<td>String</td>
		<td>	The date (month, day, and year) that the data was created. 
		<br><br>Must follow <a href="https://en.wikipedia.org/wiki/ISO_8601">ISO 8601</a> naming standards.
		</td>
	</tr>
	<tr>
		<td><strong>&lt;dcterms:modified&gt;</strong></td>
		<td>Date Modified</td>
		<td>Dublin Core</td>
		<td>Mandatory</td>
		<td>String</td>
		<td>	The date (month, day, and year) that the data was last modified. 
		<br><br>Must follow <a href="https://en.wikipedia.org/wiki/ISO_8601">ISO 8601</a> naming standards.
		</td>
	</tr>
	<tr>
		<td><strong>&lt;dctems:temporal&gt;</strong></td>
		<td>Temporal Coverage</td>
		<td>Dublin Core</td>
		<td>Mandatory</td>
		<td>String</td>
		<td>	The temporal coverage of the Wikipedia data. 
		<br><br>Must feature <strong>at least two dates</strong>, ideally formatted in ISO standards.</td>
	</tr>
	<tr>
		<td><strong>&lt;dci:subject&gt;</strong></td>
		<td>Subject</td>
		<td>DataCite</td>
		<td>Mandatory</td>
		<td>String</td>
		<td>All subjects, keywords, classification codes, or key phrases describing the data, including the contents of featured Wikipedia articles.</td>
	</tr>
	<tr>
		<td><strong>&lt;dc:accessURL&gt;</strong></td>
		<td>Public URL</td>
		<td>Dublin Core</td>
		<td>Mandatory</td>
		<td>String (must be a valid URL on the web)</td>
		<td>The Uniform Resource Locator (URL) to the page on the WikiFreaks repository where users can access the data.</td>
	</tr>
	<tr>
		<td><strong>&lt;dci:source&gt;</strong></td>
		<td>Source URL</td>
		<td>DataCite</td>
		<td>Mandatory</td>
		<td>String (must be a valid URL on the web)</td>
		<td>The Uniform Resource Locator (URL) to the original source of the data (ideally on Wikipedia).</td>
	</tr>
	<tr>
		<td><strong>&lt;ddi:license&gt;</strong></td>
		<td>License</td>
		<td>DDI</td>
		<td>Mandatory</td>
		<td>String</td>
		<td>The license that the data is shared under.
		<br><br>	Must be a valid license under <a href="https://choosealicense.com/">GitHub's "Choose a License" directory</a>.
		</td>
	</tr>
	<tr>
		<td><strong>&lt;dci:rights&gt;</strong></td>
		<td>Access Rights</td>
		<td>DataCite</td>
		<td>Mandatory</td>
		<td>String</td>
		<td>Any additional information on the rights for this resource, beyond the license itself.</td>
	</tr>
</table>

## Metadata Format:
All WikiFreaks metadata will be stored as human- and machine-readable XML (eXtensible Markup Language files. To ensure the most compatibility, the metadata is required to be in [XML 1.0](https://www.w3.org/TR/xml/). Some elements will be given an [XML Schema Instance (XSI)](https://www.w3schools.com/xml/schema_schema.asp) to provide links to the definitions in the specific namespace, adding an extra layer of authority control to our metadata. 
<br><br>
XML was picked over other machine-readable formats such as JSON because the Wikimedia Foundation itself uses XML for its WikiData project, and it will therefore be familiar to at least some of our audience.
