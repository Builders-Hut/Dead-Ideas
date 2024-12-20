# Alchemy

A database/visualization engine for chemical compounds, mapping steps, reactions, procedures, and everything that organic chemistry as a whole lacks.

## Why

Everything at the end of the day, if broken down into its simplest, is just a bunch of linked carbons, hydrogens, and whatnot. [Nile Red](https://www.youtube.com/nilered) is a YouTuber that embodies this perfectly by doing crazy experiments like [Turning styrofoam into cinnamon candy](https://www.youtube.com/watch?v=zMaTrgUKC1) and [Turning plastic gloves into hotsauce](https://www.youtube.com/watch?v=1B3Xi5L6siI).

The issue, however, is that the research that goes into this is tremendous and sometimes leads nowhere. In the world of chemistry, using rudimentary reactions like the [Wurtz reaction](https://byjus.com/chemistry/wurtz-reaction/) and others, you can create almost anything. But there isn’t a readily available solution that guides you on which reaction path to take.

During JEE preparation, we often faced questions about converting compound X to compound Y but lacked clarity on the pathway to achieve it. Even Google struggled to provide accurate results.

Hence, the idea to create a platform where users can input compound X and compound Y and receive a step-by-step chain of reactions needed to perform the transformation.

## How

### Backend Details

- **Database**:

  - Houses a comprehensive collection of chemical reactions.
  - Each reaction is stored with generalized branches to ensure applicability across various scenarios.

- **Data Structure**:

  - Reactions are treated like hashmaps where the compound acts as a key, facilitating efficient lookups and transformations.

- **Input/Output Format**:

  - Utilizes [SMILES](https://archive.epa.gov/med/med_archive_03/web/html/smiles.html) notation for the representation of chemical compounds, ensuring a standardized and widely accepted format.

- **Reaction Mapping**:

  - Implements graph algorithms to find optimal paths from compound X to compound Y, with nodes representing compounds and edges representing reactions.

- **Validation**:

  - A reaction validation system to account for the exceptions and nuances in organic chemistry, ensuring outputs are realistic and feasible.

- **Automation**:

  - Incorporates AI tools for generating and expanding the reaction database, possibly using fine-tuned models to suggest novel reactions or validate existing ones.

### Frontend Details

The frontend was developed using **Wixsite** for ease of use and rapid deployment. You can access the platform here: [Alchemy](https://astleypros333.wixsite.com/alchemy-2).

## Challenges Faced

- **Lack of Existing Reaction Databases**:

  - Few reliable sources for comprehensive reaction data.
  - Potential use of AI to prompt engineer solutions for database expansion.

- **Complexity of Chemistry**:

  - Chemistry is riddled with exceptions, making it challenging to build foolproof algorithms.

- **Niche User Base**:

  - The platform caters to a specialized audience, which may limit its adoption.

## Features

- **Compound Visualization**:

  - Drawing tools or 3D visualizations for chemical structures.

- **Reaction Explanation**:

  - Detailed insights into the mechanism of each reaction, breaking down the steps and the principles involved.

contributed by 
- [Astley](https://github.com/Astley333)
- [Sanjai]