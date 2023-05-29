# Sample Data Index:
This is a repository of sample Wikipedia data that was gathered by mixing Top 25 Reports with WikiData identifiers, to give an example of what a submission to WikiFreaks may look like.

## Proof of Conversion and Curation of Data:
Within the ["sample-data" directory](https://github.com/JoeLollo21/WikiFreaks/tree/main/sample-data), the ["Raw-Data"](https://github.com/JoeLollo21/WikiFreaks/tree/main/sample-data/Raw-Data) folder features raw data from five Top 25 reports on Wikipedia, before any authority control and data-cleaning were added to it.
<br><br>
The data was gathered, and later modified for long-term management, through the following process:
<ul>
  <li>Saving multiple Top 25 Report pages as PDFs.</li>
  <li>Using <strong>Tabula</strong> (<a href="https://tabula.technology/">"https://tabula.technology/"</a>) to convert the tables to CSV formats.</li>
  <li>The data was then cleaned for readability and given extra values, namely WikiData identifiers, using <strong>OpenRefine</strong> (<a href="https://openrefine.org/">https://openrefine.org/</a>).</li>
</ul>

## Documentation:
A [data dictionary](https://github.com/JoeLollo21/WikiFreaks/blob/main/sample-data/Sample-Data-Dictionary.csv) was created to help end-users understand what each of the dataset variables, and their sources, are. Submitters would ideally create one of these, or another form of documentation, to assist users.
