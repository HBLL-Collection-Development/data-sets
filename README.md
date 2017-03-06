## Collection development data management at BYU

For the purposes of managing our collection development data Brigham Young University, we use three branches for our data that we treat indpendently and will never merge. We have a central repository for all of our data with three branches. The first is named `raw` and contains all of our data in its raw state before we make any changes to it. Our second branch is named `normalized` and includes all of the changes we make to normalize and clean our data to get it ready for reliable analysis. Finally, our last branch is named `projects` and is used to store the projects that use our various data sets. Projects often require using multiple data sets and our `projects` branch includes a folder for each project and, subsequently, each project folder includes the transformed data sets in individual folders.

All folders within all branches of our repository include metadata about the data sets to properly document both the source of the data and the exact procedures we followed to get the data to its current state. Our Git repository structure typically looks as follows:

#### `raw` Branch

<pre>
|Data-Set-1
|    |--data
|        --raw-data-2015
|        --raw-data-2016
|        --…
|    --README.md
|    --SOURCE.md
|Data-Set-2
|    |--data
|        --raw-data-2015
|        --raw-data-2016
|        --…
|    --README.md
|    --SOURCE.md
|…
</pre>

The `raw` branch could include the following:

1. `Data-Set-Name`: Directory that is the name of the data set
2. `data`: Directory that includes all of the raw data in the data set
3. `README.md`: Readme file that describes the data set and explains the structure and meaning of the data
4. `SOURCE.md`: File with thorough documentation of the source of the data including citation information and instructions on how the data was obtained

#### `normalized` Branch

<pre>
|Data-Set-1
|    |--data
|        --normalized-data-2015
|        --normalized-data-2016
|        --…
|    --README.md
|    --RULES.md
|Data-Set-2
|    |--data
|        --normalized-data-2015
|        --normalized-data-2016
|        --…
|    --README.md
|    --RULES.md
|…
</pre>

The `normalized` branch could include the following:

1. `Data-Set-Name`: Directories that are the name of the data set
2. `data`: Directory that includes all of the cleaned and normalized data in the data set
3. `README.md`: Readme file that describes the data set and explains the structure and meaning of the data
4. `RULES.md`: File that describes all of the rules used to clean and normalize the data so that they can be replicated as the data set is updated

#### `projects` Branch

<pre>
|Project-1
|    |--data-set-1
|        --altered-data
|        --README.md
|    |--data-set-2
|        --altered-data
|        --README.md
|    --README.md
|Project-2
|    |--data-set-1
|        --altered-data
|        --README.md
|    |--data-set-2
|        --altered-data
|        --README.md
|    --README.md
|…
</pre>

The `projects` branch could include the following:

1. `Project-Name`: Directories containing the data sets used in the projects
2. `data-set`: Directories containing the data set(s) used in the project
    1. `README.md`: Readme file containing a description of how the data was altered to be used in the project
3. `README.md`: Readme file discussing the data set(s) used in the project and why they were used; will also include any metadata about the project
