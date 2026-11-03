# diffusiondatasets

Personal collection of public diffusion MRI datasets.

## Datasets with annotated bundles

### TractoInferno
- Théaud, G., Houde, J.-C., Boré, A., Rheault, F., & Descoteaux, M. (2023). *TractoInferno: A large-scale diffusion MRI tractography dataset with bundle annotations*. arXiv.
- https://openneuro.org/datasets/ds003900/versions/1.1.1
- Multi-subject in-vivo diffusion MRI dataset for tractography/bundle learning; TE/TR, voxel size, b-values, diffusion timings (δ/Δ), and FOV are provided per subject in BIDS sidecars.
- Bundle labels are distributed in the release; extraction procedure/tool/QA summary still to be completed from the dataset paper/docs (**TBD**).

### HCP105
- Van Essen, D. C., Smith, S. M., Barch, D. M., Behrens, T. E. J., Yacoub, E., & Ugurbil, K. (2013). The WU-Minn Human Connectome Project: An overview. *NeuroImage, 80*, 62-79. https://doi.org/10.1016/j.neuroimage.2013.05.041
- https://zenodo.org/records/1477956
- HCP 3T diffusion protocol: 1.25 mm isotropic, b=1000/2000/3000 s/mm², 90 directions per shell (+b0), TR ≈ 5520 ms, TE ≈ 89.5 ms; full gradient tables in HCP metadata. Typical preprocessing includes susceptibility correction (topup), eddy/motion correction, gradient-nonlinearity correction, and EPI distortion handling.
- Bundle annotations are provided in this benchmark derivative; the exact segmentation workflow/toolchain and QA protocol should be documented from the benchmark documentation (**TBD**).

### CamCAN benchmark
- Shafto, M. A., Tyler, L. K., Dixon, M., Taylor, J. R., Rowe, J. B., Cusack, R., ... Cam-CAN. (2014). The Cambridge Centre for Ageing and Neuroscience (Cam-CAN) study protocol. *BMC Neurology, 14*, 204. https://doi.org/10.1186/s12883-014-0204-1
- https://brainlife.io/pub/6a014fb3ea4d9f77d878b3cf
- Adult lifespan diffusion MRI cohort adapted into a tractography benchmark; protocol commonly reported as multi-direction single-shell dMRI (exact TE/TR, b-values, voxel size, FOV, and timing parameters should be copied from the benchmark release metadata, **TBD**).
- Bundle labels/segmentations are distributed in the benchmark package; annotation extraction procedure/tool/QA details still to be extracted from benchmark docs (**TBD**).

### HCP-YA updated benchmark
- Van Essen, D. C., Smith, S. M., Barch, D. M., Behrens, T. E. J., Yacoub, E., & Ugurbil, K. (2013). The WU-Minn Human Connectome Project: An overview. *NeuroImage, 80*, 62-79. https://doi.org/10.1016/j.neuroimage.2013.05.041
- https://brainlife.io/pub/69d5696404be87075a466ef4
- HCP-YA acquisition characteristics follow HCP 3T protocol (1.25 mm isotropic, b=1000/2000/3000 s/mm², 90 directions/shell, TR ≈ 5520 ms, TE ≈ 89.5 ms) with HCP minimal preprocessing (topup/eddy/motion + gradient nonlinearity correction).
- Harmonized bundle annotations are included; exact annotation generation toolchain and QA criteria should be added from release docs (**TBD**).

## Test-retest

### Penthera 3T
- Tax, C. M. W., Grussu, F., Kaden, E., Ning, L., Rudrapatna, U., John Evans, C., ... Jones, D. K. (2019). Cross-scanner and cross-protocol diffusion MRI data harmonisation: A benchmark database and evaluation of algorithms. *NeuroImage, 195*, 285-299. https://doi.org/10.1016/j.neuroimage.2019.01.077
- https://zenodo.org/records/2602049
- Repeated 3T dMRI sessions for harmonization/reproducibility; scanner/protocol details include TE/TR, b-values, voxel size, and diffusion timing parameters in release metadata (extract exact TE/TR/δ/Δ/FOV table from Zenodo package, **TBD**). Preprocessing in the benchmark paper includes denoising, motion/eddy/susceptibility correction, and harmonization evaluation pipelines.

### Penthera 1.5T
- Tax, C. M. W., Grussu, F., Kaden, E., Ning, L., Rudrapatna, U., John Evans, C., ... Jones, D. K. (2019). Cross-scanner and cross-protocol diffusion MRI data harmonisation: A benchmark database and evaluation of algorithms. *NeuroImage, 195*, 285-299. https://doi.org/10.1016/j.neuroimage.2019.01.077
- https://zenodo.org/records/2602022
- Repeated 1.5T dMRI sessions for cross-scanner comparison; scanner/protocol details include TE/TR, b-values, voxel size, and diffusion timing parameters in release metadata (extract exact TE/TR/δ/Δ/FOV table from Zenodo package, **TBD**). Preprocessing in the benchmark paper includes denoising, motion/eddy/susceptibility correction, and harmonization evaluation pipelines.

## Phantoms

### FiberCup (MICCAI 2015 / Neher formulations)
- Fillard, P., Poupon, C., Mangin, J.-F., Frouin, V., Clark, C. A., Le Bihan, D., ... Poupon, F. (2011). Quantitative evaluation of 10 tractography algorithms on a realistic diffusion MR phantom. *NeuroImage, 56*(1), 220-234. https://doi.org/10.1016/j.neuroimage.2011.01.032
- **TBD** (current target is to publish a cleaned-up personal version)
- Digital/simulated phantom with controlled crossings and known geometry; sequence parameters (TE/TR, b-values, voxel size, FOV) vary by formulation and should be listed per released variant (**TBD**).
- Ground-truth bundles come from phantom design; segmentation/QA are simulation-defined rather than manual labeling.

### ISMRM 2015 tractography challenge phantom
- Maier-Hein, K. H., Neher, P. F., Houde, J.-C., Côté, M.-A., Garyfallidis, E., Zhong, J., ... Descoteaux, M. (2017). The challenge of mapping the human connectome based on diffusion tractography. *Nature Communications, 8*, 1349. https://doi.org/10.1038/s41467-017-01285-x
- http://tractometer.org/ismrm2015/
- Simulated dMRI phantom for tractography evaluation; protocol typically includes multi-shell HARDI simulation with known gradient table and fixed voxel geometry (exact parameter table for b-values/TE/TR/FOV should be added from challenge files, **TBD**).
- Ground-truth streamlines/tract definitions are provided by simulation design; QA is based on geometric consistency against known tracts.

### 99 synthetic subjects
- **TBD**
- **TBD**
- Synthetic multi-subject diffusion cohort; add exact generation protocol (noise model, gradient scheme, b-values, voxel size, and preprocessing simulation steps) when source is identified (**TBD**).

## Tumors / lesions

### OpenNeuro ds004910
- **TBD** (dataset-specific citation to be added)
- https://openneuro.org/datasets/ds004910/versions/1.0.1
- In-vivo diffusion MRI with lesion/tumor relevance; extract TE/TR, b-values, voxel size, FOV, and additional modalities from BIDS sidecars/participants metadata (**TBD**). Add preprocessing details from derivatives/paper when available (**TBD**).

### BTC post-op (OpenNeuro ds002080)
- **TBD** (dataset-specific citation to be added)
- https://openneuro.org/datasets/ds002080/versions/4.0.1
- Post-operative brain tumor cohort with diffusion MRI; extract exact TE/TR, b-values, voxel size, FOV, and modality inventory from release sidecars (**TBD**). Add released preprocessing details (denoising/distortion/motion/registration pipeline) when documented (**TBD**).

### BTC pre-op (OpenNeuro ds001226)
- **TBD** (dataset-specific citation to be added)
- https://openneuro.org/datasets/ds001226/versions/5.0.1
- Pre-operative brain tumor cohort with diffusion MRI; extract exact TE/TR, b-values, voxel size, FOV, and modality inventory from release sidecars (**TBD**). Add released preprocessing details (denoising/distortion/motion/registration pipeline) when documented (**TBD**).

## b-tensor encoding

### Cardiff dataset
- **TBD**
- **TBD**
- b-tensor encoded diffusion MRI (expected LTE/PTE/STE design); add exact protocol table (b-tensor shapes, b-values, TE/TR, gradient waveform timing, voxel size, FOV) and preprocessing details from the source release (**TBD**).

### Kerkelä dataset
- Kerkelä, L., Henriques, R. N., Hall, M. G., & others. (2020). *Constrained and rotationally invariant mapping of microscopic diffusion anisotropy with diffusion-relaxation MRI*.
- **TBD**
- Tensor-valued diffusion-encoding dataset for microstructure modeling; add exact LTE/PTE/STE protocol (b-values, TE/TR, voxel size, gradient timing/waveforms, FOV) and released preprocessing steps (**TBD**).

## Multi-TE

### SciDB dataset
- **TBD**
- https://www.scidb.cn/en/detail?dataSetId=411f844eb7974da68d08569a1cb27693#p2
- Multi-echo diffusion MRI dataset; extract full TE train, TR, b-values, voxel size, FOV, and gradient scheme from dataset description/files (**TBD**). Add preprocessing/derivative steps when documented (**TBD**).

## Time-varying gradients

### 300 mT/m gradient comprehensive dataset
- Jones, D. K., Alexander, D. C., Cercignani, M., et al. (2021). Comprehensive diffusion MRI dataset for in vivo human brain microstructure mapping using 300 mT/m gradients. *Figshare collection*.
- https://springernature.figshare.com/collections/Comprehensive_diffusion_MRI_dataset_for_in_vivo_human_brain_microstructure_mapping_using_300_mT_m_gradients/5315474
- High-gradient diffusion MRI (up to 300 mT/m) with broad protocol coverage; include exact TE/TR, b-value ranges, waveform timing (δ/Δ or equivalent), voxel size, and FOV per protocol from collection files (**TBD**). Preprocessing/derivative details are provided with the release and should be copied into this entry in a follow-up pass.
