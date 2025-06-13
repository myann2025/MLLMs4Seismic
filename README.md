# MultiModal LLMs for Seismic Interpretation
1) Data Preparation for Multimodel LLMs for Seismic Interpretation
2) MLLM training

3) Test on image44_seismic.jpg

***before the training, LLama Model gives hallucination interpretation as follows,***

"
This 3D seismic cube reveals an anticline characterized by two sets of stratal patterns on opposite sides. A stratigraphic break between two layers is marked by the upper fold in the northern region. Meanwhile, the southern portion features a tilted stratigraphic break with a smaller fold and no change in reflection coefficient, indicative of an overturned anticline structure.

In contrast to the other three areas, where two different stratigraphic units are present, the center of this region only features one set of strata, likely a faulted stratigraphic unit with a major stratigraphic break at the bottom, potentially causing a subsidence or uplift.

This seismic cube provides a clear insight into the subsurface structure of the anticline, highlighting the stratigraphic changes and the presence of faults that influence the geometry of the layers.
"

***The interpretation from the finetuned model is shown below***,

"This seismic reflection image features gently dipping sedimentary layers that form a broad syncline fold structure. The reflections curve downward toward the center of the image, confirming symmetric compression and sediment accumulation in a marine environment. This type of geometry suggests a tilted crustal wedge configuration typical of regional fold-and-thrust belts.
"

***The ground truth caption is***

"This seismic image shows a broad syncline structure composed of gently dipping sedimentary layers. The reflections curve downward toward the center of the image, characteristic of compressional folding. A prominent angular unconformity at the top truncates the folded strata, indicating a major erosional surface formed after folding but before the deposition of the overlying tilted layers. The entire sequence, including the unconformity, dips slightly to the right, suggesting later regional tilting.
"

The corresponding seismic test image is shown as,

![image](https://github.com/user-attachments/assets/16d204fb-7207-4fa1-b605-34e5140dd8b7)


The training loss curves from WandB as follows,

![image](https://github.com/user-attachments/assets/c746c960-4bf3-47bc-b38c-f9a7d4ee012b)


You are welcome to use this small dataset to multimodal LLMs for seismic interpretation tests.

Please acknowledge me if you can.
