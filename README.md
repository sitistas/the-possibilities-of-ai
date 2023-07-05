# Microsoft Build After Party | The possibilities of AI

This repository was created to host the code files needed for the purposes of our Microsoft Build After Party. You can find more information in [our webpage](https://sfoteini.github.io/microsoft-build-after-party-2023)

If you want to run the demo for [Image Vector Similarity Search with Azure Computer Vision and PostgreSQL](https://github.com/sfoteini/image-vector-search-azure-postgresql), you can find the corresponding GitHub repository [here](https://github.com/sfoteini/image-vector-search-azure-postgresql), and the blog post that Foteini has created [here](https://sfoteini.github.io/blog/image-vector-similarity-search-with-azure-computer-vision-and-postgresql/)

## What is included in this demo?

- A [Jupyter notebook](vision-studio-demo.ipynb) that uses the latest feature of the Azure Cognitive Services for Vision (Computer Vision 4.0), which you can access via the [Vision Studio](https://portal.vision.cognitive.azure.com/). The services that are included in this notebook are:
  - Background removal
  - Dense Captions
  - Image Captioning
  - Object Detection
  - Image Tagging
  - Crop Suggestions
  - Face Detection
  - Text Recognition
- A [test image](images/turtle-coral-reef.jpg) that you can use to test the services.
- A [sample output image](output/sample_output.png) that you can use to compare your results with the expected ones.

## How to run the demo?

1. Sign up for a free Azure account [here](https://azure.microsoft.com/en-us/free/). If you are a student, you can also sign up for a free account [here](https://azure.microsoft.com/en-us/free/students/).
2. Create a [Cognitive Services resource in the Azure Portal](https://portal.azure.com/#create/Microsoft.CognitiveServicesAllInOne).

   **Note:** If you also want to use this for the Image Retrieval demo in the Vision Studio, you should select **East US** as the region of your resource.

3. Clone this repository: `git clone https://github.com/sitistas/the-possibilities-of-ai.git`
4. Install Python3 in your computer.
5. (Optional but recommended) Install Visual Studio Code and the Jupyter Notebook extension to run the notebook.
6. Create a file called .env in the project folder, which will contain the keys of your Cognitive Services resource. The file should look like this:

   ```.env
   'CV_ENDPOINT'=https://<COGNITIVE_SERVICES_RESOURCE_NAME>.cognitiveservices.azure.com/
   'CV_KEY'=<A 32 character string that you can find in the Keys and Endpoint section of your resource>
   ```

7. Run the notebook and enjoy!
