# WikiFreaks Metadata Profile
## Metadata Schema:
The WikiFreaks repository uses a unique, in-house metadata schema combining three standards:
<br>
- Most attributes come from the DataCite schema, which is widely used in the documentation of research data. DataCite was picked as the core schema because it was found . 
<br>
- Information on data licenses and edits made to the datasets comes from the DDI (Data Documentation Initiative) schema, primarily used for statistical and social science data. This content is not present in the DataCite schema, and we added these DDI terms because of the WikiFreaks repository’s central value of accountability for the open uploading and reuse of data.
<br>
- Temporal elements – namely for the creation and modification of data and the temporal coverage of datasets – come from the Dublin Core Metadata Initiative (DCMI) schema. These are integral to WikiFreaks’ mission to provide users with historical data on Wikipedia, and was borrowed for metadata because DataCite did not have sufficiently comprehensive indicators of time.
<br> 
Similarly, information on URLs to the data were borrowed from DCMI. Since the “accessURL” element in DCMI is more specific than DataCite’s generic “resource” element, where URLs are traditionally stored in metadata, we decided to borrow that additional element.
<br><br>
Below you will see all metadata elements in use, including potential vocabulary or standard restrictions and notes on usage. 
