# Metadata Guidance Tables (M1 – M8) 

↓ Field contents are the same as the field above; (M) (M)Mandatory
field; (A)Automatically populated field; (O)Optional field

**<span class="smallcaps">Table M-1. Process Metadata Conventions
Conventions</span>**

<table>
<tbody>
<tr class="odd">
<td><strong>Field Name</strong></td>
<td><strong>Convention</strong></td>
<td><strong>Examples</strong></td>
</tr>
<tr class="even">
<td><strong>General Information</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(M) Name[5]</td>	
<td><p>Process name based on the <strong>FLCAC naming convention;</strong> the name should reflect the product or service it represents; the product reference output is given the same name as the process name; the naming conventions are as follows:</p>
<p><strong>Base name; treatment, routes, standards; production type, location type; quantitative flow properties</strong></p>
<blockquote>
<p>The base name is a general descriptive name of the process using technical language. The technical name should be given as it is used in the respective industry or toward their customers. The standards include qualitative information about the process in technical terms (see Rules 12-17 <span class="underline">Appendix E:</span> <span class="underline">ILCD Nomenclature Rules</span> or the full <a href="http://eplca.jrc.ec.europa.eu/uploads/MANPROJ-PR-ILCD-Handbook-Nomenclature-and-other-conventions-first-edition-ISBN-fin-v1.0-E.pdf"><span class="underline">ILCD Handbook</span></a> for a list of potential descriptive terms). The quantitative process properties further specify information on process in technical quantitative term(s).</p>
</blockquote>
<p>Base name and treatment/routes/standards are mandatory; production/location type is mandatory if relevant to the process (if not, it can be ignored); the location type of availability (LCAC) is designated only if the process is not a mix; if the process is a production or consumption mix, the mix type is indicated; finally, any essential quantitative properties of the product or process should be included.</p>
<p>For consistent nomenclature, use the following guidelines:</p>
<ul>
<li><p>separate components with a semi-colon</p></li>
<li><p>separate elements within a component with a comma</p></li>
<li><p>abbreviations should be avoided</p></li>
<li><p>limit names to 220 characters</p></li>
</ul></td>
<td><p><strong>Example with 3 components</strong></p>
<p><em>Clinker; average mineral mix, at kiln, 1415 kg/m3</em></p>
<p><strong>Example with 3 components</strong><br />
<em>Transport; long-haul truck, diesel powered; trip length &gt; 200 mi</em><br />
<br />
<strong>Example with 2 components</strong><br />
<em>Scanner manufacture; Kodak Alaris i940 desktop manufacturing process</em></p></td>
</tr>
</tr>
<tr class="even">
<td>(A) Description</td>
<td><p><span class="underline">A combination of the following:</span></p>
<p><strong>1.</strong> Technology description (only introduction and PROCESS DESIGN paragraph)<br />
<strong>2.</strong> System boundaries (Boundary conditions only)</p>
<p><strong>3.</strong> Any additional details key to understanding the process (may or may not be a repeat of metadata included in other fields)</p></td>
<td><p><em>This process represents the production of "Calcium carbonate, ground, 20 micron, at plant" using average technologies for the United States from 2015-2016. The process includes three sub-processes: Quarry Operations; Transport and Plant Processing. Quarry Operations includes the following unit operations: mechanical extraction; primary crushing; screening; and intermediate storage of calcium carbonate rock (marble, limestone, or chalk). Transport includes the transport of materials from Quarry Operations to Plant Processing via barge, train, or truck. Plant processing which includes jaw crushing, washing, impact crushing, ball milling to particle size, and then classifying.</em></p>
<p><em>The system boundary includes: 1) the transport of raw materials to multiple manufacturing facilities where various subcomponents are produced; 2) the manufacture of subcomponents; 3) the transport of subcomponents to a different manufacturing plant for final assembly; 4) the assembly of subcomponents into a complete scanner; and 5) the transport of generated waste from the manufacturing facilities to a municipal solid waste landfill. The following processes and life cycle phases fall outside the system boundary: 1) packaging of the completed scanner; 2) all transport downstream of the assembly plant gate; 3) sale of product; 4) product use phase; and 5) end-of-life phase (including recycling).</em></p></td>
</tr>
<tr class="odd">
<td>(M) Category</td>
<td>The category/subcategories schema follows North American Industry Classification System (NAICS) coding. Categorize process by placing it in the proper folder in the repository process tree (using the <strong>FLCAC categorization convention</strong> as a guide); Once the openLCA data set(s) have been synced to the FLCAC Collaboration Server, the processes may be filtered by category providing a ‘process tree’ similar to that of other LCA software displays and should guide the placement of your datasets in the FLCAC categorization scheme; use the format main category (2-digit NAICS)/ (4-digit NAICS) schema (see Appendix E: 2018 NAICS United States Structure).</td>
<td><p><em>22: Utilities/2211: Electric Power Generation, Transmission and Distribution</em></p>
<p><em>31-33: Manufacturing/3253: Pesticide, Fertilizer, and Other Agricultural Chemical Manufacturing</em></p></td>
</tr>
<tr class="even">
<td><em><strong><span class="smallcaps">Table M-1. General Information Field Conventions, cont.</span></strong></em></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>Field Name</strong></td>
<td><blockquote>
<p><strong>Convention</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Examples</strong></p>
</blockquote></td>
</tr>
<tr class="even">
<td><strong>General Information, cont.</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(A) Version</td>
<td>Per the ILCD, the data set version; the first two digits indicate major updates, while the second two digits refer to minor revisions and error corrections; the final three digits are used for automatic and internal version counting during dataset development; Unless discussed in advance with the Data Curator, the value will be generated automatically by openLCA</td>
<td><em>01.00.000</em></td>
</tr>
<tr class="even">
<td>(A) UUID</td>
<td>32-digit Universally Unique Identifier (UUID) for the data set[6]</td>
<td><em>961fad56-bde2-4fbe-8895-5be03461729b</em></td>
</tr>
<tr class="odd">
<td>(A) Last change</td>
<td>The date and time when the dataset was last saved</td>
<td><em>2019-04-01T17:38:55-0600</em></td>
</tr>
<tr class="even">
<td>(M) Infrastructure process</td>
<td>Checking this box indicates that the process that produces infrastructure (i.e., inventory are only infrastructure). Leave this box unchecked if the process is not a process that produces infrastructure</td>
<td>False</td>
</tr>
<tr class="odd">
<td><strong>Quantitative reference</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(M) Quantitative reference</td>
<td>When you create a new process, this is the basis by which all the process flows are scaled; often the functional unit; the quantitative reference must be one of the process output flows; the output flows appear in a pull-down menu by default (See <span class="underline">Rule 8: “Quantitative flow properties” name field</span>, in Appendix E: ILCD Nomenclature Rules).</td>
<td><em>Scanner; Kodak Alaris i940 desktop scanner; Global supply chain; 1 unit, 1.55 kg</em></td>
</tr>
<tr class="odd">
<td><strong>Time</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(M) Start date</td>
<td>Start date for the time period that the process represents. The date format is MM/DD/YYYY</td>
<td><em>01/01/2018</em></td>
</tr>
<tr class="odd">
<td><em><strong><span class="smallcaps">Table M-1. General Information Field Conventions, cont.</span></strong></em></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><strong>Field Name</strong></td>
<td><blockquote>
<p><strong>Convention</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Examples</strong></p>
</blockquote></td>
</tr>
<tr class="odd">
<td><strong>Time, cont.</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(M) End date</td>
<td><blockquote>
<p>End date for the time period that the process represents. The date format is MM/DD/YYYY</p>
</blockquote></td>
<td><blockquote>
<p><em>12/31/2018</em></p>
</blockquote></td>
</tr>
<tr class="odd">
<td>M Description</td>
<td>Additional information regarding the temporal characteristics and period that the process represents. Examples can include the period for which the process is valid, any temporal aggregation, data collection period, seasonal/annual variations, and carbon provenance</td>
<td><em>This unit process is representative of operations from 2014-2015. Water consumption varied seasonally but was averaged over an annual period.</em></td>
</tr>
<tr class="even">
<td><strong>Geography</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(M) Location</td>
<td>The geographic area to which the unit process data were collected or refer. The FLCAC recommends that the geography reference the highest geographic resolution possible. Indicate ‘US’ unless higher geographic resolution is available. Use ISO 3166-2 code indicating the process’ geographic location if it is a US state. If the data are not a US state, also describe the locations in the geography ‘Description’ field</td>
<td><em>US-CO</em></td>
</tr>
<tr class="even">
<td>(O) KML</td>
<td>Keyhole Markup Language (KML) file which allows users to create a coordinate point, bounding box or polygon indicating the geographic area the process represents; external KML files cannot be submitted</td>
<td><em>Polygon [-77.92, 39.55… -77.92, 39.55]</em></td>
</tr>
<tr class="odd">
<td><em><strong><span class="smallcaps">Table M-1. General Information Field Conventions, cont.</span></strong></em></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><strong>Field Name</strong></td>
<td><blockquote>
<p><strong>Convention</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Examples</strong></p>
</blockquote></td>
</tr>
<tr class="odd">
<td><strong>Geography, cont.</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(M) Description</td>
<td>Description of the process' geographic representativeness and any geographic aggregation methods</td>
<td><em>This process is representative of production in the state of Colorado. Production data were aggregated across five sites ranging from eastern to western Colorado.</em></td>
</tr>
<tr class="odd">
<td><strong>Technology</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(M) Description</td>
<td>A short (i.e., 1-3 paragraphs), general description of the process intended technical scope, representativeness, and relevance. Include the following information (if applicable):<br />
<strong>1.</strong> Process design including sub-processes, unit operations, and/or other activities (anthropogenic or natural) included in the process.<br />
<strong>2.</strong> Material selection and quality.<br />
<strong>3.</strong> Operational conditions.<br />
<strong>4.</strong> A description of any fate and transport modeling</td>
<td><em>This process represents the production of "Calcium carbonate, ground, 20 microns, at plant" using average technologies for the United States from 2015-2016.<br />
<br />
The process includes three sub-processes: Quarry Operations; Transport and Plant Processing. Quarry Operations includes the following unit operations: mechanical extraction; primary crushing; screening; and intermediate storage of calcium carbonate rock (marble, limestone, or chalk). Transport includes the transport of materials from Quarry Operations to Plant Processing via barge, train, or truck. Plant processing which includes jaw crushing, washing, impact crushing, ball milling to particle size, and then classifying. Material selection and quality represent industry averages from the contiguous United States. Operational conditions represent industry averages from the contiguous United States. Fate and transport modeling was not considered for this process.</em></td>
</tr>
<tr class="odd">
<td><strong>Data quality</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(M) Process schema</td>
<td>Currently, the only default process schema for data quality available in openLCA is adapted from ecoinvent®; an agency may have their own scheme and/or other data quality schemes may be downloaded from openLCA and imported (e.g., the US EPA Data Quality system for the process schema)</td>
<td><em>US EPA Data Quality system</em></td>
</tr>
<tr class="odd">
<td><em><strong><span class="smallcaps">Table M-1. General Information Field Conventions, cont.</span></strong></em></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><strong>Field Name</strong></td>
<td><blockquote>
<p><strong>Convention</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Examples</strong></p>
</blockquote></td>
</tr>
<tr class="odd">
<td><strong>Data quality, cont.</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(M) Data quality entry</td>
<td>Selecting the “(not specified)” link opens the Pedigree matrix, in which you can select the cardinal indicators for flow reliability, temporal correlation, geographical correlation, further technological correlation, and data collection methods (i.e., completeness). For details on the data quality scheme, see the pull-down menu descriptors in openLCA or the <a href="https://cfpub.epa.gov/si/si_public_file_download.cfm?p_download_id=528687"><span class="underline">EPA 2016 Guidance Document on Data Quality Assessment for LCI Data.</span></a></td>
<td><em>(1;2;1;1;1)</em></td>
</tr>
<tr class="odd">
<td>(O) Flow schema</td>
<td>Currently, the only default flow schema for data quality available in openLCA is adapted from ecoinvent®; an agency may have their own scheme and/or other data quality schemes may be downloaded from openLCA and imported (e.g., the US EPA Data Quality system for the flow schema).</td>
<td><em>US EPA Data Quality system</em></td>
</tr>
<tr class="even">
<td>(O) Social schema</td>
<td>Currently, the only default social schema for data quality available in openLCA is adapted from ecoinvent®</td>
<td><em>ecoinvent® data quality system</em></td>
</tr>
</tbody>
</table>

###### 

***<span class="smallcaps">Table M-2. Inputs Field Conventions</span>***

<table>
<tbody>
<tr class="odd">
<td><strong>Field Name</strong></td>
<td><strong>Convention</strong></td>
<td><strong>Examples</strong></td>
</tr>
<tr class="even">
<td><strong>Inputs</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(A) Flow</td>
<td>
<strong>Elementary Flows:</strong>

Elementary flows should be named based on the <strong> FEDEFL nomenclature guidelines</strong>. For general elementary flow information see Highlights 1-14 of <span class="underline">Appendix D: FEDEFL Nomenclature Highlights</span>. See the <span class="underline">full <a href="https://cfpub.epa.gov/si/si_public_record_report.cfm?Lab=NRMRL&dirEntryId=341199">FEDEFL Guidance</a></span> for detailed conventions.

<strong>Technosphere Flows:</strong>

Flow name based on the <strong>ILCD Naming Convention</strong> (see General Information, Name Field Conventions). For general technosphere flow and for general product/process flow names, see Rules 1-19 of <span class="underline">Appendix E: ILCD Nomenclature Rules</span>. See the <span class="underline">full <a href="http://eplca.jrc.ec.europa.eu/uploads/MANPROJ-PR-ILCD-Handbook-Nomenclature-and-other-conventions-first-edition-ISBN-fin-v1.0-E.pdf">ILCD Handbook</a></span> for detailed conventions</td>
<td><em>
<strong>Elementary Flow</strong>

'Biological'

Hardwood, Resource/Biotic

<strong>Technosphere Flow</strong>

EPS virgin resin manufacture; batch suspension polymerization; industry average, at plant</em></td>
</tr>
<tr class="even">
<td>(A) Category</td>
<td>Flow category as elementary flow or detailed technosphere flow categorization based on the <strong>FLCAC Categorization Convention</strong> (see General Information, Name Field Conventions)</td>
<td><em><strong>Technosphere Flow</strong>
31-33: Manufacturing/3252: Resin, Synthetic Rubber, and Artificial Synthetic Fibers and Filaments Manufacturing</em></td>
</tr>
<tr class="odd">
<td><em><strong><span class="smallcaps">Table M-2. Inputs Field Conventions, cont.</span></strong></em></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><strong>Field Name</strong></td>
<td><blockquote>
<p><strong>Convention</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Examples</strong></p>
</blockquote></td>
</tr>
<tr class="odd">
<td><strong>Inputs, cont.</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(M) Amount</td>
<td>Flow quantity</td>
<td><em>0.484</em></td>
</tr>
<tr class="odd">
<td>(M) Unit</td>
<td>Flow unit; the openLCA software includes a set of unit groups and units; these units must be used to ensure proper data importation. If these units are not appropriate for one or more of your dataset flows, let your Data Curator know and FLCAC will assist in adding a unit to the list</td>
<td><em>kg</em></td>
</tr>
<tr class="even">
<td>(O) Costs/ Revenues</td>
<td>This field is provided for documenting Life Cycle Costing (LCC) data; the currency and costs may be provided for each flow; the costs per unit are automatically generated based on this information and flow amount</td>
<td><em>1.45 USD/kg</em></td>
</tr>
<tr class="odd">
<td>(O) Uncertainty</td>
<td>Describe flow's data uncertainty. This information is not required, but if provided it increases the process' usefulness. The distribution type, mean, and standard deviation may be provided</td>
<td><em>Normal distribution</em><br />
Mean = 0.484<br />
Standard deviation = 0.15</td>
</tr>
<tr class="even">
<td>(O) Avoided waste</td>
<td>If there is a scrap or waste flow that is utilized in your process, the flow may be listed as an input to your dataset and marked as an avoided waste</td>
<td><em>Bottle waste</em></td>
</tr>
<tr class="odd">
<td>(O) Provider</td>
<td>If the flow is produced by more than one process, you may use the drop-down menu to select a default provider.</td>
<td><em>Aluminum production; hot rolling; production mix, at plant</em></td>
</tr>
<tr class="even">
<td>(O) Data quality entry</td>
<td>Describe the flow's data quality. This information is not required, but if provided it increases the process' usefulness. The flow data quality schema must first be defined on the ‘General information’ tab to be entered for each flow in the ‘Inputs/Outputs’ tab. Currently, the only default flow schema for data quality available in openLCA is adapted from ecoinvent®; an agency may have their own scheme and/or other data quality schemes may be downloaded from openLCA and imported (e.g., the US EPA Data Quality system for the flow schema).. For details on the data quality scheme, see the pull-down menu descriptors in openLCA or the <a href="https://cfpub.epa.gov/si/si_public_file_download.cfm?p_download_id=528687"><span class="underline">EPA 2016 Guidance Document on Data Quality Assessment for LCI Data.</span></a></td>
<td><em>(1;2;1;2;4)</em></td>
</tr>
<tr class="odd">
<td>(M) Description</td>
<td>This field is required where applicable. Briefly describe the flow's relationship to the process and assumptions used to obtain the quantitative reference or data quality.</td>
<td><em>Transport to secondary processing</em></td>
</tr>
</tbody>
</table>

***<span class="smallcaps">Table M-3. Outputs Field
Conventions</span>***

<table>
<tbody>
<tr class="odd">
<td><strong>Field Name</strong></td>
<td><strong>Convention</strong></td>
<td><strong>Examples</strong></td>
</tr>
<tr class="even">
<td><strong>Outputs</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(A) Flow</td>
<td><strong>Elementary Flows:</strong>

Elementary flows should be named based on the <strong> FEDEFL nomenclature guidelines</strong>. For general elementary flow information see Highlights 1-14 of <span class="underline">Appendix D: FEDEFL Nomenclature Highlights</span>. See the <span class="underline">full <a href="https://cfpub.epa.gov/si/si_public_record_report.cfm?Lab=NRMRL&dirEntryId=341199">FEDEFL Guidance</a></span> for detailed conventions.

<strong>Technosphere Flows:</strong>

Flow name based on the <strong>ILCD Naming Convention</strong> (see General Information, Name Field Conventions). For general technosphere flow and for general product/process flow names, see Rules 1-19 of <span class="underline">Appendix E: ILCD Nomenclature Rules</span>. See the <span class="underline">full <a href="http://eplca.jrc.ec.europa.eu/uploads/MANPROJ-PR-ILCD-Handbook-Nomenclature-and-other-conventions-first-edition-ISBN-fin-v1.0-E.pdf">ILCD Handbook</a></span> for detailed conventions</td>
<td><em><strong>Elementary Flows:</strong>

'Groups of Chemicals'
Particulate matter, ≤ 10μm, Emission/Air

<strong>Technosphere Flows:</strong>

Scanner; Kodak Alaris i940 desktop scanner; Global supply chain; 1 unit, 1.55 kg</em></td>
</tr>
<tr class="even">
<td>(A) Category</td>
<td>Flow category as elementary flow or detailed technosphere flow categorization based on the <strong>FLCAC Categorization Convention</strong> (see General Information, Name Field Conventions)</td>
<td><strong>Technosphere Flow</strong>

31-33: Manufacturing/3341: Computer and Peripheral Equipment Manufacturing</em></td>
</tr>
<tr class="odd">
<td>(M) Amount</td>
<td>Flow quantity</td>
<td><em>1.55</em></td>
</tr>
<tr class="even">
<td>(M) Unit</td>
<td>Flow unit</td>
<td><em>kg</em></td>
</tr>
<tr class="odd">
<td>(O) Costs/ Revenues</td>
<td>This field is provided for documenting Life Cycle Costing (LCC) data; the currency and costs may be provided for each flow; the costs per unit are automatically generated based on this information and flow amount</td>
<td><em>15 USD/unit</em></td>
</tr>
<tr class="even">
<td>(O) Uncertainty</td>
<td>Describe flow's data uncertainty. This information is not required, but if provided it increases the process' usefulness. The distribution type, mean, and standard deviation may be provided</td>
<td><em>Normal distribution</em><br />
Mean = <em>1.55</em><br />
Standard deviation = 0<em>.44</em></td>
</tr>
<tr class="odd">
<td>(O) Avoided product</td>
<td>Used to indicate allocation has been avoided in a multi-functional process. This box should only be checked for the by-product flow(s). If the box is checked, the process avoiding the product flow must also be submitted.</td>
<td><em>Blank</em></td>
</tr>
<tr class="even">
<td><em><strong><span class="smallcaps">Table M-3. Outputs Field Conventions, cont.</span></strong></em></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>Field Name</strong></td>
<td><blockquote>
<p><strong>Convention</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Examples</strong></p>
</blockquote></td>
</tr>
<tr class="even">
<td><strong>Outputs, cont.</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(O) Data quality entry</td>
<td>Describe the flow's data quality. This information is not required, but if provided it increases the process' usefulness. The flow data quality schema must first be defined on the ‘General information’ tab to be entered for each flow in the ‘Inputs/Outputs’ tab. Currently, the only default flow schema for data quality available in openLCA is adapted from ecoinvent®; an agency may have their own scheme and/or other data quality schemes may be downloaded from openLCA and imported (e.g., the US EPA Data Quality system for the flow schema). For details on the data quality scheme, see the pull-down menu descriptors in openLCA or the <a href="https://cfpub.epa.gov/si/si_public_file_download.cfm?p_download_id=528687"><span class="underline">EPA 2016 Guidance Document on Data Quality Assessment for LCI Data.</span></a></td>
<td><em>(1;2;1;2;4)</em></td>
</tr>
<tr class="even">
<td>(M) Description</td>
<td>This field is required where applicable. Briefly (1 sentence or less) describe the flow's relationship to the process</td>
<td><em>Transport to secondary processing</em></td>
</tr>
</tbody>
</table>

***<span class="smallcaps">Table M-4. Administrative Information Field
Conventions</span>***

<table>
<tbody>
<tr class="odd">
<td><strong>Field Name</strong></td>
<td><strong>Convention</strong></td>
<td><strong>Examples</strong></td>
</tr>
<tr class="even">
<td><strong>Administrative Information</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(M) Intended application</td>
<td><p>Use one of the four Main Goal Situations below to describe how the process is intended to be used. The term, "Main Goal Situations," refers to an LCA study's primary intended purpose per the ILCD Handbook’s Detailed Guidance[7]. Additionally, you should indicate the target audience and the context for which the model was built (e.g., carbon footprint, Environmental Product Declaration (EPD), policy development, policy information, generic unit process data, etc.). Indicate the completeness level of the elementary flows such that users can interpret the correct application of LCIA methods to the dataset. If the data were originally developed and analyzed with a LCIA method, indicate the method utilized here. If these data are an update to a previously published dataset, a note should be included here.</p>
<p><strong>SITUATION A -- MICRO-LEVEL DECISION SUPPORT<br />
</strong><em>The intended application for this process is for micro-level decision support as described in Goal Situation A from the ILCD Handbook's Detailed Guidance. LCA studies with this intended application are often used to answer product-related questions. Decisions stemming from these LCA studies "are assumed to have only limited or no structural consequences outside the decision-context,...do not change available production capacity...[and do not cause] large-scale consequences in the background system or other parts of the technosphere[.]"</em><br />
<br />
<strong>SITUATION B -- MESO/MACRO-LEVEL DECISION SUPPORT<br />
</strong><em>The intended application for this process is for meso/macro-level decision support as described in Goal Situation B from the ILCD Handbook's Detailed Guidance. LCA studies with this intended application are often used to support strategic level decisions such as "raw materials strategies, technology scenarios, policy options, etc. [Such decisions] are assumed to [result in] large-scale consequences in the background system or other parts of the technosphere."</em></p>
<p><strong>SITUATION C1 -- ACCOUNTING</strong><br />
<em>The intended application for this process is for accounting purposes as described in Goal Situation C1 from the ILCD Handbook's Detailed Guidance. LCA studies with this intended application offer "purely descriptive documentation of the system under analysis (e.g., a product, sector or country), without being interested in any potential consequences on other parts of the economy.” The studies categorized under Goal Situation C1 do consider existing benefits outside the analyzed system such as recycling.</em><br />
<br />
<strong>SITUATION C2 -- ACCOUNTING</strong><br />
Same as in SITUATION C1 except LCA studies categorized under Goal Situation C2 do NOT consider existing benefits outside the analyzed system such as recycling.</p></td>
<td><p>These data are an update to the 2007 dataset with the same process name.</p>
<p><strong>SITUATION A -- MICRO-LEVEL DECISION SUPPORT<br />
</strong><em>The intended application for this process is for micro-level decision support as described in Goal Situation A from the ILCD Handbook's Detailed Guidance. These data were developed as specific, average or generic unit process LCI results for use in answering internal company product-related questions. A full inventory of environmental flows are included, thus this unit process can be used for a full range of LCIA impact categories, on the fate and transport considerations have been applied. The original study results were analyzed using the TRACI LCIA factors.</em></p></td>
</tr>
</tbody>
</table>

<table>
<tbody>
<tr class="odd">
<td><em><strong><span class="smallcaps">Table M-4. Administrative Information Field Conventions, cont.</span></strong></em></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><strong>Field Name</strong></td>
<td><strong>Convention</strong></td>
<td><strong>Examples</strong></td>
</tr>
<tr class="odd">
<td><strong>Administrative Information, cont.</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(M) Data set owner</td>
<td>Name of the agency/program that owns the dataset directly from which the process was generated. The field is populated from the list of Actors in the openLCA navigation tree. If your agency/program is not yet listed in the Actors menu, then it may be added.</td>
<td><em>National Energy Technology Laboratory</em></td>
</tr>
<tr class="odd">
<td>(M) Data generator</td>
<td>Name of the person, group of persons, or entity responsible for generating the dataset from which the process was generated. This field is also populated from the list of Actors in the openLCA navigation tree. If your person/group/entity is not yet listed in the Actors menu, then it may be added.</td>
<td><em>Timothy Skone</em></td>
</tr>
<tr class="even">
<td>(M) Data documentor</td>
<td>Name of the individual or entity that transformed the dataset into the published openLCA version of this dataset. The field is populated from the list of Actors in the openLCA navigation tree. If your person/group/entity is not yet listed in the Actors menu, then it may be added.</td>
<td><em>Timothy Skone</em></td>
</tr>
<tr class="odd">
<td>(M) Publication</td>
<td>Reference to an openLCA Source that illustrates how the processes' LCI data were developed and/or used, i.e., a foundational publication that illustrates how the data are used. The Citation should use the American Psychological Association (APA) format. The field is populated from the list of Sources in the openLCA navigation tree. If your publication is not yet listed in the Actors menu, then it may be added.</td>
<td><a href="https://www.lcacommons.gov/lca-collaboration/National_Energy_Technology_Lab/coal_extraction/dataset/SOURCE/0f6f75b5-1096-40ab-a4c9-9a6f53e802e1"><em>National Energy Technology Laboratory (NETL). 2013. Surface Coal Mining – Overburden Removal, Extraction, and Reclamation</em></a></td>
</tr>
<tr class="even">
<td>(A) Access and use restrictions</td>
<td><p>If your agency has their own data access use restrictions policy, it should be included in the published datasets. If your agency does not have a specific policy, the FLCAC default may be used (see: Data Provider’s Content License Agreement (“Agreement”)).</p>
<p>This field is populated by individual agencies and contains legal language about how the dataset may be used.</p></td>
<td><em>See Appendix A: <span class="underline">Data Use Disclaimer Agreement (“Agreement”)</span></em></td>
</tr>
<tr class="odd">
<td>(O) Project</td>
<td>Information about the project in which the data were generated. Where applicable, this field should indicate the project name, funding agency(ies), office(s) or program(s), and the grant or contract names and numbers.</td>
<td><em>This project was supported by the Biomass Research and Development Initiative, grant no. 2011-10006-30357 from the USDA National Institute of Food and Agriculture.</em></td>
</tr>
<tr class="even">
<td><em><strong><span class="smallcaps">Table M-4. Administrative Information Field Conventions, cont.</span></strong></em></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>Field Name</strong></td>
<td><strong>Convention</strong></td>
<td><strong>Examples</strong></td>
</tr>
<tr class="even">
<td><strong>Administrative Information, cont.</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(A) Creation date</td>
<td>The date and time when the dataset was published to the FLCAC. The date format is <em>MM/DD/YY HH: MM AM/PM.</em> This field will be automatically generated when the dataset is published to the FLCAC.</td>
<td><em>06/1/18 12:45 PM</em></td>
</tr>
<tr class="even">
<td>(M) Copyright</td>
<td>The openLCA software has a checkbox that will indicate whether the dataset is copyrighted. No processes published in the FLCAC are copyrighted. Leave the box unchecked</td>
<td><em>Blank</em></td>
</tr>
</tbody>
</table>

#### 

***<span class="smallcaps">Table M-5. Modeling and Validation Field
Conventions</span>***

<table>
<tbody>
<tr class="odd">
<td><strong>Field Name</strong></td>
<td><strong>Convention</strong></td>
<td><strong>Examples</strong></td>
</tr>
<tr class="even">
<td><strong>Modeling and validation</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(M) Process type</td>
<td>Indication of whether the data represent a unit or system process, where a system process is an LCI result.</td>
<td><em>Unit process</em></td>
</tr>
<tr class="even">
<td>(M) LCI method</td>
<td>Indicate whether the LCI method was attributional, consequential, input/output, hybrid, etc.</td>
<td><em>Attributional</em></td>
</tr>
<tr class="odd">
<td>(M) Modeling constants</td>
<td>State the primary assumptions used to create this process; for multi-functional processes, describe how emissions were allocated among the co-products; provide allocation factors and supporting calculations as necessary</td>
<td><em>This process was adapted from an ecoinvent® process for wood pellet manufacturing for pellets of a specific energy value. The process weight factors were adapted for the energy density of a typical US biomass fuel.</em></td>
</tr>
<tr class="even">
<td><em><strong><span class="smallcaps">Table M-5. Modeling and Validation Field Conventions, cont.</span></strong></em></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>Field Name</strong></td>
<td><strong>Convention</strong></td>
<td><strong>Examples</strong></td>
</tr>
<tr class="even">
<td><strong>Modeling and validation, cont.</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(M) Data completeness</td>
<td>A qualitative and quantitative description of missing and excluded data. This field is comprised of three elements:<br />
<br />
<strong>1. TREATMENT OF MISSING ENVIRONMENTAL DATA</strong><br />
List and describe accounting methods for missing environmental data (e.g., cut-off rules) and/or intentional environmental data omissions. As applicable, discuss missing data related to the following: air used in combustion; nutrients to/from air and soil; occupied area; particulate matter; transformed area; water withdrawal; and other directly extracted resources.<br />
<br />
<strong>2. TREATMENT OF MISSING TECHNOSPHERE DATA</strong><br />
List and describe accounting methods for missing technosphere data and/or intentional technosphere data omissions. As applicable, discuss missing data related to the following: co-production; consumption of ancillary materials such as energy, fuel, and product materials; transport; and water production or use.<br />
<br />
<strong>3. MASS BALANCE</strong><br />
Either quantify and describe the mass imbalance ((mass of material outputs - mass of material inputs)/mass of material outputs) or state, "The mass balance for this process was not calculated."</td>
<td><em><strong>TREATMENT OF MISSING ENVIRONMENTAL DATA</strong><br />
Elementary flows are cut-off at less than 1% based on environmental relevance.<br />
<br />
<strong>TREATMENT OF MISSING TECHNOSPHERE DATA</strong><br />
Intermediate flows are cut-off at less than 1% based on environmental relevance. Capital equipment is not included in this unit process.<br />
<br />
<strong>MASS BALANCE</strong><br />
The mass imbalance for this unit process is -17.87 kg (-0.72%).</em></td>
</tr>
<tr class="even">
<td>(O) Data selection</td>
<td>The principle that have been used when selecting which data to include in the process; e.g., the principle applied for choosing data sources to use for different parts of the process.</td>
<td><em>Source 1 disaggregated waste inputs and listed heating values and emission factors for the incineration; whereas, Source 2 had only heating values for waste flow inputs. Therefore, Source 2 waste heating values were excluded from the averages.</em></td>
</tr>
</tbody>
</table>

<table>
<tbody>
<tr class="odd">
<td><em><strong><span class="smallcaps">Table M-5. Modeling and Validation Field Conventions, cont.</span></strong></em></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><strong>Field Name</strong></td>
<td><strong>Convention</strong></td>
<td><strong>Examples</strong></td>
</tr>
<tr class="odd">
<td><strong>Modeling and validation, cont.</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(M) Data treatment</td>
<td>Detailed description of the methods and assumptions used to transform primary and secondary data into flow quantities through recalculating, reformatting, aggregation, or proxy data. Also includes a description of the data quality according to FLCAC convention</td>
<td><em>Primary data were taken from precise engineering specifications specific to this unit process. These data were then transformed into material and energy flows using the methodology described in Publication (2016) which is due to be released in April 2017. The Publication (2016) methodology is almost identical to the methodology described in Other Publication (2012) which is an ISO 14044 compliant, peer-reviewed LCA report of three [insert product]. Secondary data were taken from the ecoinvent® 3.2 database (Wernet et al. 2018) and the US Life Cycle Inventory Database (National Renewable Energy Laboratory 2018). The data were North American except where otherwise specified.</em></td>
</tr>
<tr class="odd">
<td><strong>Data source information</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(M) Sampling procedure</td>
<td>Detailed description of how boundary conditions were defined, how data were collected, and how uncertainty is estimated. This field is comprised of three elements:<br />
<br />
<strong>BOUNDARY CONDITIONS<br />
</strong>A description of what is included and excluded from the system boundaries.<br />
<br />
<strong>DATA COLLECTION</strong><br />
A description of how primary and/or secondary data were collected for this unit process.<br />
<br />
<strong>UNCERTAINTY ESTIMATION<br />
</strong>A description of if and how uncertainty was calculated for this process. If uncertainty was not calculated, this should be explicitly stated.</td>
<td><em><strong>BOUNDARY CONDITIONS</strong><br />
The system boundary includes: 1) the transport of raw materials to multiple manufacturing facilities where various subcomponents are produced; 2) the manufacture of subcomponents; 3) the transport of subcomponents to a different manufacturing plant for final assembly; 4) the assembly of subcomponents into a complete scanner; and 5) the transport of generated waste from the manufacturing facilities to a municipal solid waste landfill. The following processes and life cycle phases fall outside the system boundary: 1) packaging of the completed scanner; 2) all transport downstream of the assembly plant gate; 3) sale of product; 4) product use phase; and 5) end-of-life phase (including recycling).<br />
<br />
<strong>DATA COLLECTION</strong><br />
For material inputs, data collection was based on facility data provided by facilities to the National Database. Other inputs (e.g. energy; waste transport and disposal) were calculated using engineering estimates and secondary literature on the basis of quantity of input per kg of product produced.<br />
<br />
<strong>UNCERTAINTY ESTIMATION</strong><br />
Uncertainty was estimated based on engineering judgment. Material inputs had some uncertainty because they were based off of reported quantities. Other inputs (e.g. energy; waste transport and disposal) had more uncertainty.</em></td>
</tr>
<tr class="odd">
<td><em><strong><span class="smallcaps">Table M-5. Modeling and Validation Field Conventions, cont.</span></strong></em></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><strong>Field Name</strong></td>
<td><strong>Convention</strong></td>
<td><strong>Examples</strong></td>
</tr>
<tr class="odd">
<td><strong>Data source information, cont.</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(M) Data collection period</td>
<td>Time period in which the data were collected.</td>
<td><em>Secondary data were collected from 2005-2018 per Source [1] 2005, Source [2] 2010, and Source [3] 2018.</em></td>
</tr>
<tr class="odd">
<td><strong>Process evaluation and validation</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(M) Reviewer</td>
<td>Reference to the openLCA Actor who reviewed the dataset.</td>
<td><em>Robert James</em></td>
</tr>
<tr class="odd">
<td>(O) Data set other evaluation</td>
<td>Additional review information pertaining to the dataset (e.g., single or panel review, internal or third party, data entry proofreading, mass balance verification, data documentation review, etc.).</td>
<td><em>The LCA study that produced this unit process was critically reviewed per ISO 14040 and 14044 standards by Ph.D. Office of Strategic Energy Analysis &amp; Planning, National Energy Technology Laboratory.</em></td>
</tr>
<tr class="even">
<td><strong>Sources</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(M) Sources</td>
<td>Reference to the publication(s), agency(ies), program(s), and/or entity(ies) from which data were obtained (from the openLCA Sources pull-down menu; add a new one, if the desired reference is not available).</td>
<td><p><em>Illinois Department of Natural Resources. 2006. Annual Statistical Report, 2006</em></p>
<p><em>Bucyrus International. 2008b. Continuous Miner Specifications.</em></p>
<p><em>Bucyrus International. 2008a. Continuous Miners: The Range.</em></p>
<p><em>National Energy Technology Laboratory (NETL). 2010. Continuous coal miner; Manufacture; At underground mine; 563 kW</em></p>
<p><em>National Renewable Energy Laboratory (2016). US Life Cycle Inventory Database.Sustainable Solutions Corporation. (2016). IMA-NA Calcium Carbonate Life Cycle Assessment</em></p>
<p><em>US Department of Commerce Census of Manufacturers’ Shipments, Inventories &amp; Orders, May 2018 Report</em></p>
<p><em>BTS – Bureau of Transportation Statistics Commodity Flow Survey of 2012.</em></p></td>
</tr>
</tbody>
</table>

***<span class="smallcaps">Table M-6.</span>***
***<span class="smallcaps">Global Parameters Field Conventions</span>***

<table>
<tbody>
<tr class="odd">
<td><strong>Field Name</strong></td>
<td><strong>Convention</strong></td>
<td><strong>Examples</strong></td>
</tr>
<tr class="even">
<td><strong>General Information</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(O) Name</td>
<td>Parameter name. Parameter names have the following restrictions: no spaces; no special characters; no more than 255 characters</td>
<td><em>belt_length</em></td>
</tr>
<tr class="even">
<td>(O) Description</td>
<td>Brief description of how and why the parameter was developed.</td>
<td><em>Total conveyor belt length in meters.</em></td>
</tr>
<tr class="odd">
<td><strong>Additional Information (used when creating new Global Parameters in the openLCA navigation tree)</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(O) Type</td>
<td><p>Designates whether the parameter is an input or dependent parameter type:</p>
<p><strong>Input parameters</strong>: are only valid in the process/LCIA method/product system in which they are defined and saved</p>
<p><strong>Dependent parameters</strong>: include input or global parameters in their formula</p></td>
<td><em>Input</em></td>
</tr>
<tr class="odd">
<td>(O) Amount/Value</td>
<td>The default numeric value for the database</td>
<td><em>73.32</em></td>
</tr>
<tr class="even">
<td>(O) Uncertainty</td>
<td>Describe parameter's uncertainty. This information is not required, but if available and provided, increases the dataset's clarity.</td>
<td><em>Triangle distribution</em><br />
Minimum = <em>50</em><br />
Mode = <em>75</em><br />
Maximum = <em>100</em></td>
</tr>
<tr class="odd">
<td>(O) Dependent Parameter Formula</td>
<td>Parameter formulas have the following rules:<br />
<strong>1.</strong> Operators include "+","-","*","/".<br />
<strong>2.</strong> Must use the parameter names as named in the ‘Parameters’ tab or otherwise already defined as global parameters in the openLCA database navigator.<br />
<strong>3.</strong> Maximum of 255 characters and no units so the unit should be added to the ‘Description’ field<br />
<strong>4.</strong> More complex functions are possible (such as using Booleans and regular expressions), but are not documented and described here.<br />
<strong>5.</strong> Additional information on parameter functions can be found in the openLCA user manual</td>
<td><em>(cold_st_wt*belt_length)+tail_pulley+drive_pulley</em></td>
</tr>
</tbody>
</table>

***<span class="smallcaps">Table M-7. Process Parameters</span>***

<table>
<tbody>
<tr class="odd">
<td><strong>Field Name</strong></td>
<td><strong>Convention</strong></td>
<td><strong>Examples</strong></td>
</tr>
<tr class="even">
<td><strong>Input &amp; Dependent Parameters</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(O) Name</td>
<td>Parameter name. Parameter names have the following restrictions: no spaces; no special characters; no more than 255 characters</td>
<td><em>belt_length</em></td>
</tr>
<tr class="even">
<td>(O) Description</td>
<td>Brief description of how and why the parameter was developed.</td>
<td><em>Total conveyor belt length in meters.</em></td>
</tr>
<tr class="odd">
<td><strong>Additional Information</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(O) Amount/Value</td>
<td>The default numeric value for the database</td>
<td><em>73.32</em></td>
</tr>
<tr class="odd">
<td>(O) Uncertainty</td>
<td>Describe parameter's uncertainty. This information is not required, but if available and provided, increases the dataset's clarity.</td>
<td><em>Triangle distribution</em><br />
Minimum = <em>50</em><br />
Mode = <em>75</em><br />
Maximum = <em>100</em></td>
</tr>
<tr class="even">
<td>(O) Dependent Parameter Formula</td>
<td>Parameter formulas have the following rules:<br />
<strong>1.</strong> Operators include "+","-","*","/".<br />
<strong>2.</strong> Must use the parameter names as named in this ‘Parameter’ tab in the process or otherwise already defined as global parameters in the openLCA database navigator under ‘Indicators and parameters/Global parameters.’<br />
<strong>3.</strong> Maximum of 255 characters and no units so the units should be added to the ‘Description’ field<br />
<strong>4.</strong> More complex functions are possible (such as using Booleans and regular expressions), but are not documented and described here.<br />
<strong>5.</strong> Additional information on parameter functions can be found in the openLCA user manual</td>
<td><em>(cold_st_wt*belt_length)+tail_pulley+drive_pulley</em></td>
</tr>
</tbody>
</table>

***<span class="smallcaps">Table M-8. Allocation Field Conventions (Only
for Multi-Functional Processes)</span>***

<table>
<tbody>
<tr class="odd">
<td><strong>Field Name</strong></td>
<td><strong>Convention</strong></td>
<td><strong>Examples</strong></td>
</tr>
<tr class="even">
<td><strong>Physical &amp; economic allocation (Mandatory only for physical &amp; economic allocation)</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>(M) Default method</td>
<td>Pull-down menu allows designation of no method or causal, economic, or physical allocation methods for multi-functional processes</td>
<td><em>Physical</em></td>
</tr>
<tr class="even">
<td>(A) Product</td>
<td>Is the first reference flow by default; the primary product and co-products must have the same flow property</td>
<td><p><em>bark (0.3 kg)</em></p>
<p><em>wood (1.00 kg)</em></p></td>
</tr>
<tr class="odd">
<td>(A) Physical</td>
<td>Allocation factors are based on the physical (e.g., mass or energy) ratio of the product flows; the ratio for the product will be 1.0 for a single-output process; for multi-output processes, the ‘Calculate default values’ button will automatically calculate the ratios based on the default (reference) flow property</td>
<td><p><em>0.23076923076923075</em></p>
<p><em>0.7692307692307692</em></p></td>
</tr>
<tr class="even">
<td>(A) Economic</td>
<td>Allocation factors are based on the economic value of the product flows; the ratio of the product will be 1.0 for a single-output process; for multi-output processes, an economic flow property must first be added to each product flow; then, the ‘Calculate default values’ button will automatically calculate the ratios based on the economic value of the product flows</td>
<td><p><em>0.1071428571485712</em></p>
<p><em>0.8928571428571428</em></p></td>
</tr>
<tr class="odd">
<td><strong>Causal allocation (Mandatory only for causal allocation)</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>(A) Flow</td>
<td>Lists the process flow outputs and inputs</td>
<td><em>Green lumber</em></td>
</tr>
<tr class="odd">
<td>(A) Direction</td>
<td>Indicates whether the flow is a process input or output</td>
<td><em>Output</em></td>
</tr>
<tr class="even">
<td>(A) Category</td>
<td>Indicates the flow category</td>
<td><em>Forestry and logging/Logging</em></td>
</tr>
<tr class="odd">
<td>(A) Amount</td>
<td>The amounts are automatically calculated given the causal allocation ratio entered in the columns to the right of the amounts (i.e., for each product/by-product); the ratios are added manually</td>
<td><em>Bark 0.4 kg; Wood 0.6 kg for a causal ratio of 0.4 to 0.6</em></td>
</tr>
</tbody>
</table>

#### 

#### <span class="smallcaps">Social aspects field conventions: Social aspects are not addressed in this handbook.</span>
