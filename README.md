# Auido-viusal-multimodal-dysarthria-assessment---Master-thesis
The codes for the master thesis  -- Audio-Visual Fusion for Multimodal Automatic Dysarthria Assessment with Speaker-Disjoint Split in Mandarin

# Introduction:
This thesis investigates a multimodal ADA framework that integrates both audio and video modalities to assess Mandarin-speaking individuals with dysarthria. Drawing on the Mandarin Subacute Stroke Dysarthria Multimodal (MSDM) database, we build a bimodal system using pre-trained encoders for each modality and apply transfer learning to adapt them to the dysarthric domain. A speaker-disjoint dataset split is employed to reflect realistic clinical scenarios, ensuring that the system is evaluated on unseen speakers. To fuse the extracted features, we explore various feature-level fusion strategies to fuse the extracted features, including linear, MLP-based, and attention-based methods. The codes are written using Python in Jupyter notebooks.


# Dataset:
The thesis works on the Open-Access database: Mandarin Subacute Stroke Dysarthria Multimodal (MSDM). To get access, go to the website:  https://huanraozhineng1.github.io/MSDM/

J. Liu et al., "The Open-Access Mandarin Subacute Stroke Dysarthria Multimodal (MSDM) Database for Intelligent Assessment," 2024 IEEE 14th International Symposium on Chinese Spoken Language Processing (ISCSLP), Beijing, China, 2024, pp. 131-135, doi: 10.1109/ISCSLP63861.2024.10799983. keywords: {Pathology;Databases;Speech recognition;Stroke (medical condition);Neurorehabilitation;Object recognition;Labeling;Mandarin;Subacute stroke;Dysarthria;Audio-video database}

# Files
Five Jupyter notebook files.

1. audio_spectrogram_extract.ipynb: The mel-spectrograms of the audio data are extracted and stored in a single file.
2. encoder_finetuning.ipynb:  The mel-spectrograms are loaded, and the video frames are obtained. The mel-spectrograms are passed through a 2D ResNet18. The video frames are passed through a 3DResNet18.
3. embedding_extract.ipynb: The audio embeddings are extracted from mel-spectrograms by the audio encoder. The video embeddings are extracted from video frames by the video encoder.
4. classification.ipynb: The extracted embeddings are fused and then passed through a variety of classifiers.
5. best-performance-analysis.ipynb: The classification of the best performance is presented. The detailed classification is analyzed. 








