| Property             | Description (from [DCAT-US v3.0](https://doi-do.github.io/dcat-us/) documentation)                                                                                                       | Context provided relevant to generative AI-related data retrieval                                                                                                                               |
|--------------------------|------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Access Restriction](https://doi-do.github.io/dcat-us/#distribution-access_restriction)       | An indication of whether there are access restrictions on the data                                                     | Ensures responsible access to sensitive historical records. Enhances transparency, aiding researchers and authorized users in understanding and navigating access parameters for archived materials |
| [Data Dictionary](https://doi-do.github.io/dcat-us/#dataset-describedBy)          | Specifies a data dictionary or schema that defines fields (variables, dimensions, measures, attributes) in the dataset | Important both for parsing dataset correctly and provides context to improve quality of patterns learned and model output                                                                           |
| [Identifier](https://doi-do.github.io/dcat-us/#dataset-identifier)               | Unique identifier for the dataset                                                                                      | Helps disambiguate different datasets; promotes transparency and data consistency                                                                                                                   |
| [Keyword](https://doi-do.github.io/dcat-us/#dataset-keyword)                  | Keywords describing the dataset                                                                                        | Helpful to summarize larger focus of dataset; can help with finding/searching/crawling for new relevant data by developers and other users                                                          |
| [Licensing](https://doi-do.github.io/dcat-us/#distribution-license)                | This property refers to the license under which the dataset is made available                                          | Helps ensure users and automated systems parse data licenses accurately                                                                                                                             |
| [Publisher](https://doi-do.github.io/dcat-us/#dataset-publisher)                | The entity responsible for making the dataset available                                                                | Important for understanding and citing of data sources, linking other context to dataset                                                                                                            |
| [Rights](https://doi-do.github.io/dcat-us/#dataset-rights)                   | This property refers to a statement that specifies rights associated with the dataset                                  | Helps ensure users and automated systems parse data rights accurately                                                                                                                               |
| [Temporal Coverage](https://doi-do.github.io/dcat-us/#dataset-temporal-coverage)        | The time period the dataset covers                                                                                     | Important for training models with relevant temporal data and increases likelihood of models returning timely/relevant results to users                                                             |
| [Update / Modification Date](https://doi-do.github.io/dcat-us/#dataset-update-modification-date) | The most recent date on which the dataset was changed or modified                                                      | Helps model developers access/update relevant information                                                                                                                                           |

*Table 2.1: Mandatory and recommended DCAT-US v3.0 properties that are recommended by this guidance*

| Property      | Description (from [DCAT-US v3.0](https://doi-do.github.io/dcat-us/) documentation                                               | Context provided relevant to generative AI-related data retrieval                                                                             |
|---------------|----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| [Documentation](https://doi-do.github.io/dcat-us/#dataset-documentation) | A page or document containing more information about the dataset                             | Helps model developers easily identify additional relevant context/metadata about dataset                                                     |
| [Has Version](https://doi-do.github.io/dcat-us/#dataset-hasVersion)   | Indicates a related dataset that is a version, edition, or adaptation of the current dataset | Helps identify raw versus derived datasets and disambiguate different data versions                                                           |
| [Language](https://doi-do.github.io/dcat-us/#dataset-language)      | Natural language used for textual metadata of the dataset                                    | Helps ensure metadata are parsed correctly; helps users find language-specific resources to improve models for English and non-English models |
| [Provenance](https://doi-do.github.io/dcat-us/#dataset-provenance)    | A statement about the lineage of the dataset, including any changes in ownership and custody | Helps model developers access/update relevant information. Written language especially helpful context for LLM model training                 |
| [Version](https://doi-do.github.io/dcat-us/#dataset-version)       | The version name or identifier of the dataset                                                | Helps model developers access/update relevant information                                                                                     |
| [Version Notes](https://doi-do.github.io/dcat-us/#dataset-versionNotes) | A description of the differences between this and previous versions of the dataset           | Helps model developers access/update relevant information                                                                                     |

*Table 2.2: Optional DCAT-US v3.0 properties that are recommended by this guidance*

<table>
  <caption>
    <h4>
      Table 1: Utilization of Commerce open data in generative AI systems
    </h4>
  </caption>
  <thead>
    <tr>
      <th>Process</th>
      <th>Definition</th>
      <th>As it relates to Commerce data</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Training</th>
      <td>Using large-scale data to train<br>foundation models</td>
      <td>Commerce's public data provides a rich source of structured<br>and unstructured data to improve accuracy and versatility<br>of generative AI models</td>
    </tr>
    <tr>
      <th>Testing and<br>Validation</th>
      <td>Assessing model performance to<br>ensure reliability, accuracy, and<br>fairness</td>
      <td>Commerce data offers diverse datasets for testing, allowing<br>the detection of biases and errors in models across many <br>domains</td>
    </tr>
    <tr>
      <th>Fine-Tuning</th>
      <td>Refining pre-trained models to <br>improve precision for specific<br>tasks</td>
      <td>Commerce datasets can be used to fine-tune models for<br>tasks like economic forecasting and climate prediction, <br>improving model relevance and performance</td>
    </tr>
    <tr>
      <th>Data Retrieval<br>&amp; Real-Time<br>Responses</th>
      <td>Enabling AI systems to access<br>and integrate data in response to<br>real-time queries</td>
      <td>Commerce data can be retrieved in real-time through<br>methods like Retrieval-Augmented Generation (RAG),<br>ensuring users receive the most up-to-date and accurate<br>information</td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th></th>
      <th>
        <div>Guideline 1.1</div>
        <div>Provide comprehensive context about data assets in documentation</div> 
      </th>
      <th>
        <div>Guideline 1.2</div>
        <div>Maximize the availability and accessibility of documentation</div> 
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Best Practices</th>
      <td>
        <div>1.1.1 Provide helpful characteristics of open data within documentation</div>
        <br>
        <div>1.1.2 Implement persistent identifiers</div>
        <br>
        <div>1.1.3 Update documentation with each data release and use version control</div>
        <br>
        <div>1.1.4 Provide version controlled open-source code for data processing</div>
      </td>
      <td>
        <div>1.2.1 Provide documentation in human and machine-readable formats</div>
        <br>
        <div>1.2.2 Use open-source software and formats, where appropriate</div>
      </td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th></th>
      <th>
        <div>Guideline 2.1</div>
        <div>Publish comprehensive and structured data and metadata</div> 
      </th>
      <th>
        <div>Guideline 2.2</div>
        <div>Maximize the availability and accessibility of data and metadata</div> 
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Best Practices</th>
      <td>
        <div>2.1.1 Include generative AI-relevant information in metadata at the dataset level</div>
        <br>
        <div>2.1.2. Add comprehensive variable-level metadata for machine understandability</div>
        <br>
        <div>2.1.3 Publish metadata aligned with common, or accepted, metadata schemas and standards</div>
        <br>
        <div>2.1.4 Use standard missing data values within data and metadata</div>
        <br>
        <div>2.1.5 Ensure consistent and unambiguous file naming conventions</div>
      </td>
      <td>
        <div>2.2.1 Produce data and metadata in machine-readable formats</div>
        <br>
        <div>2.2.2 Data should be available in common open data formats</div>
        <br>
        <div>2.2.3 Use file structures that reduce structural ambiguity</div>
        <br>
        <div>2.2.4 When possible, both raw and derived data versions should be made available</div>
      </td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th></th>
      <th>
        <div>Guideline 3.1</div>
        <div>Disseminate open data in consistent formats</div> 
      </th>
      <th>
        <div>Guideline 3.2</div>
        <div>Store open data in easily retrievable locations</div> 
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Best Practices</th>
      <td>
        <div>3.1.1 Large datasets should be compressed or easily downloadable</div>
        <br>
        <div>3.1.2 Compress large data files using open-source and language agnostic file formats</div>
        <br>
        <div>3.1.3 Include long-form written documentation in data publications</div>
      </td>
      <td>
        <div>3.2.1 Offer a range of modalities for retrieving data, minimally by RESTful API and direct download</div>
        <br>
        <div>3.2.2 Data websites should be regularly updated and easily crawlable</div>
      </td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th></th>
      <th>
        <div>Guideline 4.1</div>
        <div>Publish comprehensible open data rights and permissions in accessible and accepted formats</div> 
      </th>
      <th>
        <div>Guideline 4.2</div>
        <div>Develop and update data licenses and usage policies collaboratively</div> 
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Best Practices</th>
      <td>
        <div>4.1.1 Explicitly define and publish generative AI-related open data usage policies in a machine-readable format</div>
        <br>
        <div>4.1.2 Include a robots.txt file at the root of Commerce websites</div>
        <br>
        <div>4.1.3 Include comprehensive rights related metadata for responsible and trustworthy AI</div>
        <br>
        <div>4.1.4 Distinguish between open data licenses (e.g. ODL) and copyright licenses (e.g. CCBY)</div>
      </td>
      <td>
        <div>4.2.1 Develop and update data licenses and usage policies collaboratively throughout Commerce</div>
        <br>
        <div>4.2.2 Adopt consistent language and metadata structure around licensing and usage for Commerce's open data</div>
      </td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th></th>
      <th>
        <div>Guideline 5.1</div>
        <div>Prepare open data for high quality data retrieval</div> 
      </th>
      <th>
        <div>Guideline 5.2</div>
        <div>Continuously evaluate open data for accuracy</div> 
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Best Practices</th>
      <td>
        <div>5.1.1 Indicate data quality in dataset metadata</div>
        <br>
        <div>5.1.2 Automate AI-ready data quality control</div>
        <br>
        <div>5.1.3 Prime APIs for high-quality data retrieval</div>
      </td>
      <td>
        <div>5.2.1 Develop benchmarking datasets for AI/ML application domains</div>
        <br>
        <div>5.2.2 Guide generative AI's responses to Commerce related prompts</div>
        <br>
        <div>5.2.3 Collaborate with developers of generative AI applications to ensure authoritative open data are prioritized</div>
      </td>
    </tr>
  </tbody>
</table>

<table>
  <caption>
    <h4>
      Figure 5: An example question and ideal response with an example API call using the American Community Survey data
    </h4>
  </caption>
  <thead>
    <tr>
      <th>Type of Question or Prompt</th>
      <th>Example Question or Prompt</th>
      <th>Ideal Response</th>
      <th>What to Avoid</th>
      <th>Relevant Census API Call</th>
      <th>Relevant Data in Response</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Population Data</td>
      <td>"What is the population of Suitland, MD?"</td>
      <td>Provide users with the source and data of the statistic (e.g. "The U.S. Census Bureau's 2022 American Community Survey estimated the population of Suitland, Maryland to be around 25,839.")</td>
      <td>Portraying estimates as counts, being vague about the source and date of the statistic</td>
      <td>https://api.census.gov/data/2022/acs/acs5/profile?get=group(DP05)&ucgid=1600000US2475725</td>
      <td>"DP05_0001E" is "25839"</td>
    </tr>
  </tbody>
</table>
