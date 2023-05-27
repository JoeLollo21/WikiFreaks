# WikiFreaks Metadata Profile
## Metadata Schema:
The WikiFreaks repository uses a unique, in-house metadata schema combining three standards:
<br>
- Most attributes come from the DataCite schema, which is widely used in the documentation of research data. DataCite was picked as the core schema because it was found . 
- Information on data licenses and edits made to the datasets comes from the DDI (Data Documentation Initiative) schema, primarily used for statistical and social science data. This content is not present in the DataCite schema, and we added these DDI terms because of the WikiFreaks repository’s central value of accountability for the open uploading and reuse of data.
- Temporal elements – namely for the creation and modification of data and the temporal coverage of datasets – come from the Dublin Core Metadata Initiative (DCMI) schema. These are integral to WikiFreaks’ mission to provide users with historical data on Wikipedia, and was borrowed for metadata because DataCite did not have sufficiently comprehensive indicators of time. Similarly, information on URLs to the data were borrowed from DCMI. Since the “accessURL” element in DCMI is more specific than DataCite’s generic “resource” element, where URLs are traditionally stored in metadata, we decided to borrow that additional element.
<br><br>
<p>Below you will see all metadata elements in use, including potential vocabulary or standard restrictions and notes on usage.</p>

## Metadata Elements:
<table>
	<tr>
		<th>Element</th>
		<th>Common Name</th>
		<th>Namespace</th>
		<th>Status</th>
		<th>Encoding</th>
		<th>Definition<br>and Rules</th>
		<th>Example</th>
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
		<td>&lt;dci:creator&gt;Lollo, Joe&lt;/dci:creator&gt;</td>
	</tr>
</table>
(just copy and paste the table when it’s transferred to Markdown)

## Metadata Format:
All WikiFreaks metadata will be stored as human- and machine-readable XML (eXtensible Markup Language files. To ensure the most compatibility, the metadata is required to be in [XML 1.0](https://www.w3.org/TR/xml/). Some elements will be given an [XML Schema Instance (XSI)](https://www.w3schools.com/xml/schema_schema.asp) to provide links to the definitions in the specific namespace, adding an extra layer of authority control to our metadata. 
<br><br>
XML was picked over other machine-readable formats such as JSON because the Wikimedia Foundation itself uses XML for its WikiData project, and it will therefore be familiar to at least some of our audience.
