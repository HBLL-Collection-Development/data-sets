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
