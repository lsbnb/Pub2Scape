# Pubtator2CytoScape
We have developed a Python tool called Pubtator2CytoScape, which is designed to parse the output of Pubtator. Pubtator2CytoScape extracts various BioConcept items (e.g., genes, diseases, chemicals, species) and calculates the frequency of each BioConcept pair (e.g., gene-gene, gene-chemical, chemical-disease) based on their co-appearance in publications. The resulting network, composed of these BioConcept items, can be imported into Cytoscape for visualization and further network analyses.

Currently, Pubtator2CytoScape is in the beta version stage. We are actively working on optimizing the program and aim to create a user-friendly graphical interface to replace the current command-line version. The current design of Pub2Cyto, named "pubtator2cytoscape_v6," can be executed using the "-i" option for the Pubtator output and the "-w" option for the frequency of each BioConcept pair.
>python pubtator2cytoscape_v5.py -i <input_pubtator_file> -w <cut_weight> 

For those keywords not identified as "bioconcepts/ NER" in pubtator, we will provide a new function, -c <custom_file>, to allow users to add their own "NER" and calculate the frequency among NERs and customized ones for visualization in Cytoscape.

Meanwhile, we also plan to implement the standalone website as a docker image with a build-in network viewer to allow researchers to perform the analysis without IT burden. All the codes developed by this project will be free and open to the public.  
