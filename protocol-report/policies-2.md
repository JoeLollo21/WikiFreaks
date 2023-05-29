# Data Transfer and Transformation Policies:
WikiFreaks is an open-access repository exploring the cultural history of Wikipedia, through which researchers may contribute or borrow data which catalogs  en.Wikipedia.org’s Top 25 reports, classifying each with unique identifiers and WikiData’s authority control system.
<br><br>
The following is a set of policies establishing WikiFreaks’ procedures regarding collected or deposited data: 

## Transfer Policy:
As stated in WikiFreaks’ [Collection Policy](https://github.com/JoeLollo21/WikiFreaks/blob/main/protocol-report/policies.md), depositing data within WikiFreaks requires approval by WikiFreaks administrators prior to its uploading. Please refer to the Collection Policy for additional deposit information, such as necessary contact information, affiliations and permissions, as well as additional descriptive data required for metadata collection—including a record of any cleaning, anonymization, or modification made to the data post-collection.
<br><br>
Apart from this, data must be: 
<ul>
  <li>Uploaded to its GitHub, following an email screening process. Contributors must be registered users on GitHub.</li>
  <li>Tabular data. <strong>Non-tabular datais not accepted and will not be checked.</strong></li>
  <li>In a non-proprietary file format, such as .CSV (preferred), .TSV, or .XLSX. <strong>Proprietary spreadsheet formats, such as .XLS, will not be accepted.</strong></li>
  <li>Approved by repository administrators after authenticity checks, which will cross-examine raw data from the Wikimedia foundation with any cleaning, anonymization, or modification packaged with submitted data.</li>
  <li>Free of any confidential, sensitive, or private information. Any and all contact information, including the affiliations of users or curators, is to be provided in a preliminary email. Personal information not originating from any Top 25 Report provided in tabular data will be deleted before files are approved.</li>
  <li>Accompanied by metadata containing contact information, date of modification and upload, a brief summary of process concerning curated data, and a short statement of purpose. The metadata will remain private to the creators of WikiFreaks other than to create demographic statistics of contributions.</li>
</ul>

## Transformation Policy:
Please refer to the [Collection Policy](https://github.com/JoeLollo21/WikiFreaks/blob/main/protocol-report/policies.md) for information on data ingestion, and preferred file formats. 
<br><br>
Data transformed by WikiFreaks will be:
<ul>
  <li>Tabular when presented to end-users, prioritizing delimited comma separated value files.</li>
  <li>Tabular when transferred and stored, where all non-proprietary spreadsheet files are acceptable.</li>
  <li>Recorded change-by-change through GitHub’s history of commits. Major changes just as updating data or changing versions must be recorded in a separate portion of the .README file, as well as noted in an “last updated” field for recorded metadata.</li>
  <li>Normalized data will feature blank spaces where [NULL] values are concerned.</li>
</ul>
