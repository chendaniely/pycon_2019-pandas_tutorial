---
layout: default
---

2. [Tidy Data][2]
	- Tidy Data
		1. Each variable forms a column.
		2. Each observation forms a row.
		3. Each type of observational unit forms a table
	- Dirty Data
		1. Column headers are values, not variable names.
		2. Multiple variables are stored in one column.
		3. Variables are stored in both rows and columns.
		4. Multiple types of observational units are stored in the same table.
		5. A single observational unit is stored in multiple tables.
1. [A Quick Guide to Organizing Computational Biology Projects][1]
	1. Project Templates
3. [Best Practices for Scientific Computing][3]
	1. Write programs for people, not computers.
	2. Let the computer do the work.
	3. Make incremental changes.
	4. Don't repeat yourself (or others).
	5. Plan for mistakes.
	6. Optimize software only after it works correctly.
	7. Document design and purpose, not mechanics.
	8. Collaborate.
4. [Good enough practices in scientific computing][4]
	1. Data management
	2. Software
	3. Collaboration
	4. Project organization
	5. Keeping track of changes
	6. Manuscripts
5 [Project Templates][5] (in R) by Dan:

```
project
|
|- data             # raw and primary data, are not changed once created
|  |
|  |- project_data  # subfolder that links to an encrypted data storage container
|  |  |
|  |  |- original   # raw data, will not be altered
|  |  |- working    # intermediate datasets from src code
|  +  +- final      # datasets used in analysis
|
|- analysis /       # any programmatic code
|  |- user1         # user1 assigned to the project
|  +- user2         # user2 assigned to the project
|
|- output           # all output and results from workflows and analyses
|  |- figures/      # graphs, likely designated for manuscript figures
|  |- pictures/     # diagrams, images, and other non-graph graphics
|  +- analysis/     # generated reports for (e.g. rmarkdown output)
|
|- README.md        # the top level description of content
|
|- Makefile         # Makefile, if applicable
|- .gitignore       # git ignore file
+- project.Rproj    # RStudio project
```

[1]: https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1000424
[2]: http://vita.had.co.nz/papers/tidy-data.html
[3]: https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001745
[4]: https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005510
[5]: https://chendaniely.github.io/sdal/2017/05/30/project_templates/
