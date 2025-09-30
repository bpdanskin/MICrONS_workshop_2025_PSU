# MICrONS_workshop_2025_PSU
MICrONS Workshop produced for Puget Sound University class NRSC490a, Fall 2025: Advanced Topics in neuroscience. 

This is an introduction to data access, programmatic tools, and general analysis for the MICrONS dataset. For more, see [tutorial.microns-explorer.org](https://tutorial.microns-explorer.org)


## MICrONS dataset tutorial: Functional connectomics spanning multiple areas of mouse visual cortex
Presented by Bethanny Danskin

The MICrONS dataset is a large functional connectomics dataset with dense calcium imaging and electron microscopy based cell reconstruction over one cubic millimeter of mouse visual cortex. All neurons were automatically reconstructed and all synapses detected.
Subsequent proofreading in this volume yielded reconstructions that include complete dendritic trees for all ~70 thousand neurons as well the local and inter-areal axonal projections of a subset of neurons that map up to thousands of cell-to-cell connections per neuron.
Functional measurements and connectivity can be related for ~12 thousand neurons which were coregistered between the calcium and EM volumes.
In this tutorial, we introduce the dataset, as well as both interactive and programmatic tools to analyze it.

The tutorial will contain examples of how to access: annotations, connectivity, segmentation, meshes, and neuron-skeletons.

Manuscript describing the dataset: [Functional connectomics spanning multiple areas of mouse visual cortex](https://www.nature.com/articles/s41586-025-08790-w)

## Dataset introduction

#### Neuroglancer: data visualization and exploration

Workshop introduction example: https://spelunker.cave-explorer.org/#!gs://microns-static-links/mm3/layer5_thick_tufted.json

Neuroglancer navigation instructions at [MICrONS Explorer Tools](https://www.microns-explorer.org/ngl-instructions)

More curated neuroglancer examples available at [the MICrONS Explorer Gallery](https://www.microns-explorer.org/gallery-mm3)

#### DashApps: interactive online analysis

Browse the data tables, such as cell type classifications with the [Table Viewer](https://minnie.microns-daf.com/dash/datastack/minnie65_public/apps/table_viewer/?datastack=%22minnie65_public%22). Documentation and use examples are here [Table Viewer Overivew](https://tutorial.microns-explorer.org/dash-table-viewer.html)

Query and visualize synaptic connectivity of neurons with the [Connectivity Viewer](https://minnie.microns-daf.com/dash/datastack/minnie65_public/apps/connectivity/?anno-id=%22%22&id-type=%22root_id%22&mat-version=1507&cell-type-table-dropdown=%22%22&datastack=%22minnie65_public%22). Documentation and use examples are here [Connectivity Viewer Overivew](https://tutorial.microns-explorer.org/dash-connectivity.html)



### Programmatic Access: using the Connectome Annotation Versioning Engine (CAVE) ecosystem

This repository includes curated Data Access examples and tutorials. To work in your local environment, clone the repo and create a new virtual environment withe the _environment_microns2025.yml_ file. 

Aleternately, you can run each notebook in __Google Colab__ by accessing the github urls, or clicking the following links:
1. [MICrONS General Data Access](https://colab.research.google.com/github/bpdanskin/MICrONS_workshop_2025_PSU/blob/main/code/colab_MICrONS_data_access.ipynb)
2. [MICrONS Advanced Neuroglancer Tools](https://colab.research.google.com/github/bpdanskin/MICrONS_workshop_2025_PSU/blob/main/code/MICrONS_advanced_nglui.ipynb)
3. [MICrONS Downloading meshes](https://colab.research.google.com/github/bpdanskin/MICrONS_workshop_2025_PSU/blob/main/code/MICrONS_mesh_access.ipynb)

(requires GMail or other Google-related account). Google Colab lets you run executable notebooks in the cloud with minimal setup.


#### Further reading relevant to the demonstration

Cell Type Model: [Perisomatic ultrastructure efficiently classifies cells in mouse cortex. Elabaddy et al.]([https://www.biorxiv.org/content/10.1101/2022.07.20.499976v2](https://www.nature.com/articles/s41586-024-07765-7))

Layer 5 ET Cell Type Paper: [The synaptic architecture of layer 5 thick tufted excitatory neurons in mouse visual cortex. Bodor et al.](https://www.nature.com/articles/s41586-024-07765-7)

Martinotti Cell Type Paper: [Connectomics of predicted Sst transcriptomic types in mouse visual cortex. Gamlin et al.](https://www.nature.com/articles/s41586-025-08805-6)

Data Infrastructure: [CAVE: Connectome Annotation Versioning Engine. Dorkenwald et al.](https://www.nature.com/articles/s41592-024-02426-z)

### Dataset documentation

More complete documentation that includes the above information as well as guides to interacting with meshes, skeletons, and imagery, [can be found online at the MICrONS Tutorial webpages](https://tutorial.microns-explorer.org/).

### Credits

Tutorial material prepared by Bethanny Danskin.
Full MICrONs project credits can be found at [MICrONs Explorer](https://www.microns-explorer.org).
