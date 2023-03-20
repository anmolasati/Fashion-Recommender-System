This project develops a fashion recommendation system for window shopping using a dataset of 16K apparel images from an e-commerce platform. The system displays four images at a time, allowing users to select one or more they like. Based on their choices and past interactions, it suggests the next set of images, continuing the process until the user decides to stop.

The recommendation approach combines exploration and exploitation through a dynamic alpha parameter:

    Exploitation: Utilizes MobileNetV2 embeddings to identify visually similar images.
    Exploration: Randomly selects images from the least viewed options.
    Epsilon smoothing refines recommendations by incorporating the user’s past selections within the same session. 
