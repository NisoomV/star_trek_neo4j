
# Star Trek Neo4j Database

This repository contains resources for building and exploring a Star Trek-themed graph database in Neo4j. The database uses data from STAPI (Star Trek API) and focuses on entities such as characters, episodes, and organizations. The project includes two Jupyter notebooks to load data into a Neo4j instance and SVG files generated from the database.

## Contents

- `Load_Episodes.ipynb`: A Jupyter notebook that loads Star Trek episode data into the Neo4j database.
- `Load_rest.ipynb`: A Jupyter notebook that loads additional data, such as characters and organizations, into the Neo4j database.
- `Emmisary.svg`: A graph visualization showing relationships between characters and episodes centered around the episode "Emissary."
- `KlingonEmpire.svg`: A graph visualization depicting the structure and key members of the Klingon Empire.
- `README.md`: Documentation for the repository.

## Requirements

- **Python 3.x**
- **Jupyter Notebook**
- **Neo4j Database** (Community or Enterprise edition)
- **Py2neo** (Python library for interacting with Neo4j)
- **STAPI** (Star Trek API - data source)

## Setup Instructions

1. **Install Neo4j**: Follow the instructions on [Neo4j's website](https://neo4j.com/download/) to install the Neo4j database.
2. **Set Up Neo4j Credentials**: Update the connection details in the notebooks to match your Neo4j setup (default is `bolt://localhost:7687` with username `neo4j`).
3. **Install Required Python Libraries**:
   ```bash
   pip install py2neo requests
4. **Run the notebooks:**
- Open Load_Episodes.ipynb and Load_rest.ipynb in Jupyter Notebook.
- Run each notebook to populate the Neo4j database with data from STAPI.

## Project Overview

This project creates a Neo4j graph database with the following entities:

-   **Character**: Nodes representing Star Trek characters.
-   **Episode**: Nodes representing episodes where characters appear.
-   **Organization**: Nodes representing organizations like the Klingon Empire.
-   **Title**: Node representing titles such as Grand Negus.

### Relationship Types

The database uses several relationship types:

-   **APPEARS_IN**: Connects characters to episodes they appear in.
-   **PART_OF**: Connects characters or organizations to larger organizations (e.g., a character belonging to the Klingon Empire).
-   **NEXT_MISSION**: Sequential connection between episodes to illustrate mission progress.
-   **Various blood relations**: Connects family members or other relations together.

## Graphs

![Emissary.svg](https://github.com/NisoomV/star_trek_neo4j/blob/4c169a3fcd4d142a1f41099a40b0395524cc7f95/Emmisary.svg)
![KlingonEmpire.svg](https://github.com/NisoomV/star_trek_neo4j/blob/4c169a3fcd4d142a1f41099a40b0395524cc7f95/KlingonEmpire.svg)

