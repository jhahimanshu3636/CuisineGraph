# CuisineGraph

**CuisineGraph** is an ambitious project dedicated to exploring the rich and diverse world of recipes, cuisines, and ingredients through the power of graph databases, specifically Neo4j. By representing culinary data in a graph structure, we aim to uncover fascinating patterns, relationships, and insights that can be leveraged for various applications, from recommendation systems to culinary explorations.

## Project Objectives

1. **Projecting Recipes**: Representing recipes as nodes within a graph, including their ingredients, steps, and other attributes.
2. **Mapping Cuisines**: Categorizing recipes into various cuisines and linking them to their characteristic ingredients and flavors.
3. **Connecting Ingredients**: Understanding the relationships between ingredients, their co-occurrences in recipes, and their roles in different cuisines.

## Data Preparation and Ingestion

### Formatting the Data

We ensure our data is in a format that can be easily processed and ingested into Neo4j. Key data files include:
- `indian_food_dataset.csv`: Contains recipe information such as recipe name, translated instructions, total time taken, ingredient count, and cuisine.
- `processed_ingridients_df.csv`: Lists ingredients used in each recipe, linking them to the respective recipe names and detailing the ingredient quantities.

### Preprocessing the Data

To ensure consistency and accuracy, we clean, normalize, and validate our data:
- **Data Cleaning**: Removing duplicates, correcting typos, and standardizing units of measurement.
- **Normalization**: Ensuring consistent naming of ingredients across all recipes.
- **Validation**: Checking for missing or inconsistent data and filling gaps where possible.

### Defining the Schema

Our Neo4j schema includes:
- **Nodes**: `Recipe`, `Ingridient`, and `Cusine`.
- **Relationships**: `HAS_INGRIDIENT` (between `Recipe` and `Ingridient` nodes) and `HAS_CUISINE` (between `Recipe` and `Cusine` nodes).

### Ingesting Data into Neo4j

We use Python and the Neo4j driver to ingest data in batches. Key functions include:
- **add_recipe**: Ingests recipe nodes.
- **add_ingridient_node**: Ingests ingredient nodes.
- **add_ingridient_relation**: Establishes relationships between recipes and ingredients.
- **add_cuisine_node**: Ingests cuisine nodes.
- **add_cuisine_relation**: Establishes relationships between recipes and cuisines.

## Conclusion

CuisineGraph aims to revolutionize the way we understand and interact with culinary data. By harnessing the power of graph databases, we offer an exciting journey into the intricate web of flavors and cuisines that define our gastronomic experiences.

Stay tuned as we continue to explore and analyze the fascinating connections within the world of recipes and cuisines!

---

**Note:** For detailed code and further explanations, please refer to the project files and documentation.

## Connect with Me

For more information and updates, feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/your-linkedin-profile).
