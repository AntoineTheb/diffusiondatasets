# diffusiondatasets

## Datasets with annotated bundles

### TractoInferno

- [OpenNeuro](https://openneuro.org/datasets/ds003900/versions/1.1.1) · [Download options](https://docs.openneuro.org/user_guide.html#viewing-and-downloading-a-dataset).
- Paper: [Poulin et al., 2022](https://doi.org/10.1038/s41597-022-01833-1).
- 284 participants; up to 30 bundles. Preprocessed DWI, T1w, fODFs, peaks and tractograms.
- Six 3T protocols; native resolution 1.75–2.3 mm; retained b=700 or 1000 s/mm²; TE=70–93 ms, TR=1800–9200 ms.
- TractoFlow preprocessing; TOPUP omitted. Four tracking methods, RecoBundlesX extraction and manual QC.
- Annotation methods: [RecoBundles](https://doi.org/10.1016/j.neuroimage.2017.07.015), [RecoBundlesX](https://savoirs.usherbrooke.ca/handle/11143/17255).

### HCP105

- [Tracts ZIP](https://zenodo.org/records/1477956/files/HCP105_Zenodo_NewTrkFormat.zip) · [DWI (HCP login + terms)](https://balsa.wustl.edu/project?project=HCP_YA).
- Papers: [Van Essen et al., 2013](https://doi.org/10.1016/j.neuroimage.2013.05.041) (cohort); [Sotiropoulos et al., 2013](https://doi.org/10.1016/j.neuroimage.2013.05.057) (acquisition).
- 105 participants, 72 manually curated bundles.
- 3T; 1.25 mm isotropic; b=1000/2000/3000 s/mm², 90 directions/shell; TE/TR=89.5/5520 ms; δ/Δ=10.6/43.1 ms; in-plane FOV 210×180 mm.
- HCP minimal preprocessing. MSMT-CSD, iFOD2, TractQuerier/WMQL, filtering and manual corrections.
- Annotation paper: [TractSeg — Wasserthal et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.07.070).

### Cam-CAN288

- [Brainlife (login + data agreement)](https://brainlife.io/pub/6a014fb3ea4d9f77d878b3cf).
- Papers: [Taylor et al., 2017](https://doi.org/10.1016/j.neuroimage.2015.09.018); [Shafto et al., 2014](https://doi.org/10.1186/s12883-014-0204-1).
- 288 participants, ages 18–87; 61 bundles.
- 3T Trio; 2 mm isotropic; b=1000/2000 s/mm², 30 directions/shell + 3 b0; TR=9100 ms; TE=104 ms in the original protocol, 106 ms in the benchmark paper; FOV 192×192 mm.
- Denoising, Gibbs correction, susceptibility/motion/eddy correction and registration. Benchmark inputs resampled to 1.25 mm.
- Bundles: ACT, modified WMQL, automated outlier rejection and tract masks.
- Annotation paper: [Kwon et al., 2026](https://doi.org/10.64898/2026.07.30.741597) (preprint).

### HCP-YA benchmark / HCP1057

- [Brainlife (login + HCP access)](https://brainlife.io/pub/69d5696404be87075a466ef4).
- Papers: [Van Essen et al., 2013](https://doi.org/10.1016/j.neuroimage.2013.05.041); [Sotiropoulos et al., 2013](https://doi.org/10.1016/j.neuroimage.2013.05.057).
- 1057 participants; 61 bundles. Preprocessed DWI, fODFs/peaks, streamlines and masks.
- HCP 3T protocol: 1.25 mm isotropic; b=1000/2000/3000 s/mm², 90 directions/shell; TE/TR=89.5/5520 ms; δ/Δ=10.6/43.1 ms.
- HCP minimal preprocessing. Same automated bundle workflow as Cam-CAN288.
- Annotation paper: [Kwon et al., 2026](https://doi.org/10.64898/2026.07.30.741597) (preprint).

## Test–retest

### Penthera 3T

- [TAR.GZ (download check blocked by Zenodo)](https://zenodo.org/records/2602049/files/Penthera_3T.tar.gz).
- Dataset: [Paquette, Gilbert & Descoteaux, 2019](https://doi.org/10.5281/zenodo.2602049).
- 13 participants, 6 scans each: 2 sessions × 3 scans.
- Philips Ingenia 3T; 2 mm isotropic; b=300/1000/2000 s/mm² with 8/32/60 directions; 7 b0 + reverse-phase b0; TE/TR=95/5615 ms. T1w at 1 mm.
- Processing reference: [TractoFlow — Théaud et al., 2020](https://doi.org/10.1016/j.neuroimage.2020.116889).

### Penthera 1.5T

- [TAR.GZ (download check blocked by Zenodo)](https://zenodo.org/records/2602022/files/Penthera_1.5T.tar.gz).
- Dataset: [Chamberland et al., 2019](https://doi.org/10.5281/zenodo.2602022).
- 10 participants, 4 scans each: two scans 10 minutes apart, repeated 2 days later.
- Siemens Magnetom 1.5T; 2 mm isotropic; b=1000 s/mm², 64 directions + 1 b0; reverse-phase b0; TE/TR=98/11000 ms. T1w at 1 mm.
- Processing reference: [TractoFlow — Théaud et al., 2020](https://doi.org/10.1016/j.neuroimage.2020.116889).

## Phantoms

### FiberCup

- [Physical phantom ZIP](https://tractometer.org/data/fibercup/all_data_3x3x3_no_rois_mask.zip) · [MICCAI 2015 TAR.GZ](https://www.nitrc.org/frs/download.php/9858/MICCAI_2015_NiftiNrrd.tar.gz) · [Fiberfox ZIP](https://www.nitrc.org/frs/download.php/5796/RecreatedFiberCup.zip).
- Physical phantom paper: [Fillard et al., 2011](https://doi.org/10.1016/j.neuroimage.2011.01.032).
- Simulation papers: [Fiberfox — Neher et al., 2014](https://pubmed.ncbi.nlm.nih.gov/24323973/); [Neher et al., 2015](https://doi.org/10.1007/978-3-319-24553-9_6).
- Physical phantom: MICCAI 2009; 3T Trio, twice-refocused EPI; 3 mm isotropic, 64×64×3; b=650/1500/2000 s/mm², 64 directions per b-value per repetition; TE=77/94/102 ms respectively, TR=5000 ms. Two acquisitions and their average.
- MICCAI 2015 simulation: 3 mm isotropic, 64×64×3; 30 directions at b≈1000 s/mm² + 1 b0.
- References: 16 manually drawn trajectories for the original physical challenge; simulation input fibers for digital variants.
- Scoring: [Tractometer — Côté et al., 2013](https://doi.org/10.1016/j.media.2013.03.009).

### ISMRM 2015 tractography challenge

- [DWI + reverse b0 ZIP](https://scil.usherbrooke.ca/ismrm2015/ISMRM_2015_Tracto_challenge_data_with_reversed_phase_v1_0.zip) · [Original references TAR.GZ](https://scil.usherbrooke.ca/ismrm2015/scoring_data_tractography_challenge.tar.gz) · [2023 references ZIP](https://scil.usherbrooke.ca/ismrm2015/scoring_data_Renauld2023.zip).
- Paper: [Maier-Hein et al., 2017](https://doi.org/10.1038/s41467-017-01285-x).
- Fiberfox simulation; 2 mm isotropic; 32 directions at b=1000 s/mm² + 1 b0; TE=108 ms. Reverse-phase b0, T1-like image and field map also available.
- 25 original reference bundles; 21 scored bundles in the 2023 revision.
- Annotation/scoring paper: [Renauld et al., 2023](https://doi.org/10.1038/s41598-023-28560-w).

### 99 simulated brains

- [Full dataset ZIP (403 GB)](https://doi.dkfz.de/10.6097/DKFZ/IR/E230/20200511_1.zip) · [One-participant ZIP (4.1 GB)](https://zenodo.org/records/4139626/files/899885.zip).
- Dataset: [Neher & Maier-Hein, 2020](https://doi.org/10.6097/e230-20200511_1).
- Methods: [Neher & Maier-Hein, ISMRM 2021](https://cds.ismrm.org/protected/21MProceedings/PDFfiles/3406.html).
- 99 HCP-derived participants; 71 reference bundles each; simulated T1w/T2w and DWI.
- Clinical: 2.5 mm, 32 directions at b=1000 s/mm² + 1 b0. Intermediate: 2 mm, 30 directions/shell at b=1000/2000/3000 s/mm² + 9 b0. HCP-like: 1.25 mm, 90 directions/shell at the same b-values + 18 b0.
- Each protocol has versions with and without added artifacts; both include Gaussian noise. TractSeg/MITK reference bundles, Fiberfox simulation.

## Tumors / lesions

### OpenNeuro ds004910

- [OpenNeuro ds004910](https://openneuro.org/datasets/ds004910/versions/1.0.1) · [Download options](https://docs.openneuro.org/user_guide.html#viewing-and-downloading-a-dataset).
- Paper: [Wu et al., 2024](https://doi.org/10.1038/s41597-024-03013-9).
- 20 participants: 18 with lesions, 2 controls. Raw and processed DWI, T1w and FLAIR.
- Philips Ingenia CX 3T; 1.5 mm isotropic; b=400/800/1600/3200 s/mm² with 4/8/8/16 directions + 4 b0 per TE; TR=4000 ms.
- TE=75–135 ms in 10-ms steps; δ=19.9–49.9 ms and Δ=35.9–65.9 ms in 5-ms steps. TE and diffusion timing change together; TE coverage varies by participant.
- Denoising, motion/eddy/bias correction, alignment across TEs and ANTs distortion correction using a synthetic T2-like image.
- Tissue labels: [SynthSeg](https://doi.org/10.1016/j.media.2023.102789) and FreeSurfer parcellations.

### BTC post-op

- [OpenNeuro ds002080](https://openneuro.org/datasets/ds002080/versions/4.0.1) · [Download options](https://docs.openneuro.org/user_guide.html#viewing-and-downloading-a-dataset).
- Paper: [Aerts et al., 2022](https://doi.org/10.1038/s41597-022-01806-4).
- 29 participants: 7 glioma, 12 meningioma, 10 controls; patients scanned approximately 6 months after surgery.
- 3T Trio; 2.5 mm isotropic; b=700/1200/2800 s/mm² with 16/30/50 diffusion-weighted volumes + 6 b0; 2 reverse-phase b0; TE/TR=110/8700 ms.
- T1w, resting-state fMRI, clinical/cognitive data and connectome derivatives. Manual/semi-automatic tumor masks and disconnection masks; methods in the dataset paper.

### BTC pre-op

- [OpenNeuro ds001226](https://openneuro.org/datasets/ds001226/versions/5.0.1) · [Download options](https://docs.openneuro.org/user_guide.html#viewing-and-downloading-a-dataset).
- Paper: [Aerts et al., 2022](https://doi.org/10.1038/s41597-022-01806-4).
- 36 participants: 11 glioma, 14 meningioma, 11 controls; 29 have post-op follow-up.
- 3T Trio; 2.5 mm isotropic; b=700/1200/2800 s/mm² with 16/30/50 diffusion-weighted volumes + 6 b0; 2 reverse-phase b0; TE/TR=110/8700 ms.
- T1w, resting-state fMRI, clinical/cognitive data and connectome derivatives. Manual/semi-automatic tumor masks and disconnection masks; methods in the dataset paper.
- Connectome pipeline: denoising, Gibbs correction, TOPUP/EDDY, registration, MSMT-CSD, ACT and SIFT. [Processing code](https://github.com/BrainModes/TVB-empirical-data-pipeline).

## b-tensor encoding

### Cardiff

- [B-tensor data ZIP](https://ndownloader.figshare.com/files/49921407).
- Paper: [Afzali et al., 2021 — SPHERIOUSLY?](https://doi.org/10.1016/j.neuroimage.2021.118183).
- 2 participants; 3T Connectom, 300 mT/m gradients; 3 mm isotropic; TE=88 ms.
- Archive: 439 LTE + 439 PTE + 182 STE volumes per participant, including 31 b0; separate reverse-phase b0. Nominal b-values extend to 12000 s/mm² for all three encodings.
- Delivered grid 70×70×42; the archive's grid and shell inventory differ from the paper's protocol description.

### Kerkelä

- [Tensor-valued data ZIP](https://zenodo.org/records/14479946/files/tensor-valued_data.zip).
- Dataset: [Kerkelä, 2024](https://doi.org/10.5281/zenodo.14479946).
- Acquisition-design reference: [Morez et al., 2023](https://doi.org/10.1002/hbm.26175).
- 1 participant; 3T Prisma; 2×2×2.1 mm grid; TE/TR=91/4200 ms.
- LTE: b=100/800/2000 s/mm², 10/64/20 volumes. PTE: b=100/800 s/mm², 6/10 volumes. STE: b=2000 s/mm², 30 volumes. Combined: 146 volumes including 6 b0; separate reverse-phase b0.
- Raw/preprocessed DWI, T1-MPRAGE, T2-FLAIR, bval/bvec/bten files and processing script. MP-PCA, Gibbs correction, TOPUP/EDDY and BET.

## Multi-TE

### SciDB

- [Science Data Bank files](https://www.scidb.cn/en/detail?dataSetId=411f844eb7974da68d08569a1cb27693#p2) · [Example DWI](https://china.scidb.cn/download?fileId=0b7375a05224c7d713f16118e9c461f1).
- Paper: [Wongkornchaovalit et al., 2025](https://doi.org/10.1038/s41597-025-05544-1).
- 3 participants; raw and preprocessed data; 3T Prisma; 2.5 mm isotropic; FOV 210×210 mm, 48 slices.
- TE=62/72/82/92/102/112/122/132 ms, with repeats at 62 and 132 ms; TR=5800 ms.
- b=700/2000 s/mm², 30 directions/shell; 4 b0 per acquisition, 2 AP + 2 PA. Fixed δ/Δ=15.2/25.2 ms across TE and b.
- MP-PCA, TOPUP/EDDY and FLIRT across TEs, with b-vector rotation.

## Diffusion-time variation / strong gradients

### MGH Connectome Diffusion Microstructure Dataset

- [Participant ZIPs](https://springernature.figshare.com/collections/Comprehensive_diffusion_MRI_dataset_for_in_vivo_human_brain_microstructure_mapping_using_300_mT_m_gradients/5315474) · [Participant 001 ZIP](https://ndownloader.figshare.com/files/30789970).
- Paper: [Tian et al., 2022](https://doi.org/10.1038/s41597-021-01092-6).
- 26 participants, 7 same-day rescans after repositioning.
- 3T Connectome, 300 mT/m gradients; pulsed-gradient LTE; 2 mm isotropic; FOV 216×216 mm; TE/TR=77/3800 ms; δ=8 ms, Δ=19/49 ms.
- 16 shells spanning b=50–17800 s/mm²; 32 directions below b=2400, 64 otherwise. 800 diffusion-weighted volumes + 50 b0; 5 reverse-phase b0.
- Preprocessed magnitude DWI, T1w, masks and FreeSurfer derivatives; real-valued DWI for 14 participants. Gradient-nonlinearity correction and TOPUP/EDDY, including slice-to-volume correction.
