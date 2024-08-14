# SynCom_SpentMedia
All files related to the spent media project using the Koskella Lab's 16 Synthetic Community and _P. syringae pv. tomato DC3000_.

## File Descriptions & Uses

### SM Processing.Rmd

My master R markdown file was used when drafting my code, running stat tests, generating figures, and more. With no prior experience in coding (any language) I learned what I needed this year from my mxntor, lab mates, and the internet. Any respectful tips, suggestions, edits, etc. are more than welcome.

### plate_maps.xlsx

This Excel sheet contains all the plate maps used across the project. 'plate_map1' and 'plate_map2' are the master maps and any additional maps were made in response to errors or changes to the wells as needed.

### Spent Media Catalogue.xlsx

This Excel sheet has basic information about the Syncom & details the system used to generate and store all the spent media (SM) types. The sheet includes: time and date each SM started and ended, how each SM was filtered, where each SM was stored, and what bacterial cultures are in each SM type.

### Heatmap_SingleSpent_NoVal.pdf

This is a heatmap that summarizes a portion of the data across the whole community made by Tiffany N. Baraseh. It can be read as how each bacterial strain (x-axis) grew in the SM of the other community members (y-axis) about its growth in fresh media (well color). The calculations were done using the following formula: Growth Factor = (Growth<sub>Spent</sub> - Growth<sub>Fresh</sub>)/(Growth<sub>Fresh</sub>).
- Growth<sub>Spent</sub> is the AUC of a bacteria in a specific SM type.
- Growth<sub>Fresh</sub> is the AUC of a bacteria's baseline growth in fresh media.

The more blue a cell color, the more positive its growth factor is in that SM, and vice versa with the yellow-red cells. The code for this figure was done by Tiffany; I will include it in the 'SM Processing.Rmd' file once I get it.

### Bacterial Data Folder

This folder contains all the raw kinetic readings for each bacteria across their two plates for the 3 days they were measured. The 'plater' files are formatted according to the plater R package guidelines found [here](https://cran.r-project.org/web/packages/plater/vignettes/plater-basics.html) to help with dataset formatting. P1 and P2 are for a bacteria's plate 1 and plate 2 respectively. Plate maps are the same as the xlsx file but in csv format for the R code to function properly.
