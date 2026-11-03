# diffusiondatasets

Personal collection of public diffusion MRI datasets.

> Notes:
> - This is a working list. Please verify references against each dataset's official citation guidance.
> - For entries where a paper or direct download URL is still unclear, the item is marked **TBD**.

## Datasets with annotated bundles

### TractoInferno
- Théaud, G., Houde, J.-C., Boré, A., Rheault, F., & Descoteaux, M. (2023). *TractoInferno: A large-scale diffusion MRI tractography dataset with bundle annotations*. arXiv.
- https://openneuro.org/datasets/ds003900/versions/1.1.1
- Multi-subject in-vivo diffusion MRI dataset curated for tractography and bundle-level analyses (scanner/protocol fields should be read from BIDS sidecars in the release).
- White-matter bundles are provided as tractography labels for supervised/benchmark use.

### HCP105
- Van Essen, D. C., Smith, S. M., Barch, D. M., Behrens, T. E. J., Yacoub, E., & Ugurbil, K. (2013). The WU-Minn Human Connectome Project: An overview. *NeuroImage, 80*, 62-79. https://doi.org/10.1016/j.neuroimage.2013.05.041
- https://zenodo.org/records/1477956
- HCP 3T diffusion protocol: 1.25 mm isotropic voxels, 3 shells (b=1000/2000/3000 s/mm²), 90 directions per shell (+b0), TR ≈ 5520 ms, TE ≈ 89.5 ms; commonly distributed with HCP minimal diffusion preprocessing (susceptibility, eddy/motion, gradient nonlinearity corrections).
- Bundle annotations are provided for tractography benchmarking workflows.

### CamCAN benchmark
- Shafto, M. A., Tyler, L. K., Dixon, M., Taylor, J. R., Rowe, J. B., Cusack, R., ... Cam-CAN. (2014). The Cambridge Centre for Ageing and Neuroscience (Cam-CAN) study protocol. *BMC Neurology, 14*, 204. https://doi.org/10.1186/s12883-014-0204-1
- https://brainlife.io/pub/6a014fb3ea4d9f77d878b3cf
- Adult lifespan diffusion MRI cohort adapted into a tractography benchmark format (exact TE/TR, b-values, and voxel geometry should be read from release metadata).
- Bundle labels/segmentations are distributed through the benchmark package.

### HCP-YA updated benchmark
- Van Essen, D. C., Smith, S. M., Barch, D. M., Behrens, T. E. J., Yacoub, E., & Ugurbil, K. (2013). The WU-Minn Human Connectome Project: An overview. *NeuroImage, 80*, 62-79. https://doi.org/10.1016/j.neuroimage.2013.05.041
- https://brainlife.io/pub/69d5696404be87075a466ef4
- Updated benchmark based on HCP Young Adult diffusion MRI (1.25 mm isotropic, multi-shell b=1000/2000/3000 s/mm²; HCP-style minimal diffusion preprocessing).
- Harmonized bundle annotations are provided for tractography evaluation.

## Test-retest

### Penthera 3T
- Tax, C. M. W., Grussu, F., Kaden, E., Ning, L., Rudrapatna, U., John Evans, C., ... Jones, D. K. (2019). Cross-scanner and cross-protocol diffusion MRI data harmonisation: A benchmark database and evaluation of algorithms. *NeuroImage, 195*, 285-299. https://doi.org/10.1016/j.neuroimage.2019.01.077
- https://zenodo.org/records/2602049
- Repeated diffusion MRI sessions at 3T for repeatability and harmonization analyses (see release files for scanner-specific TE/TR, Δ/δ, b-values, and voxel geometry).

### Penthera 1.5T
- Tax, C. M. W., Grussu, F., Kaden, E., Ning, L., Rudrapatna, U., John Evans, C., ... Jones, D. K. (2019). Cross-scanner and cross-protocol diffusion MRI data harmonisation: A benchmark database and evaluation of algorithms. *NeuroImage, 195*, 285-299. https://doi.org/10.1016/j.neuroimage.2019.01.077
- https://zenodo.org/records/2602022
- Repeated diffusion MRI sessions at 1.5T for repeatability/scanner-comparison studies (see release files for scanner-specific TE/TR, Δ/δ, b-values, and voxel geometry).

## Phantoms

### FiberCup (MICCAI 2015 / Neher formulations)
- Fillard, P., Poupon, C., Mangin, J.-F., Frouin, V., Clark, C. A., Le Bihan, D., ... Poupon, F. (2011). Quantitative evaluation of 10 tractography algorithms on a realistic diffusion MR phantom. *NeuroImage, 56*(1), 220-234. https://doi.org/10.1016/j.neuroimage.2011.01.032
- **TBD** (current target is to publish a cleaned-up personal version)
- Synthetic/phantom diffusion data with known fiber geometry and controlled crossings.
- Ground-truth pathways are defined by phantom design.

### ISMRM 2015 tractography challenge phantom
- Maier-Hein, K. H., Neher, P. F., Houde, J.-C., Côté, M.-A., Garyfallidis, E., Zhong, J., ... Descoteaux, M. (2017). The challenge of mapping the human connectome based on diffusion tractography. *Nature Communications, 8*, 1349. https://doi.org/10.1038/s41467-017-01285-x
- http://tractometer.org/ismrm2015/
- Simulated phantom with known fiber tracts for controlled tractography evaluation.
- Ground-truth streamlines/tract definitions are provided by the simulation framework.

### 99 synthetic subjects
- **TBD**
- **TBD**
- Synthetic multi-subject diffusion cohort; exact protocol parameters still to be confirmed.

## Tumors / lesions

### OpenNeuro ds004910
- **TBD** (dataset-specific citation to be added)
- https://openneuro.org/datasets/ds004910/versions/1.0.1
- In-vivo diffusion MRI with tumor/lesion relevance (TE/TR, b-values, voxel size, and preprocessing steps should be read from dataset sidecars/derivatives).

### BTC post-op (OpenNeuro ds002080)
- **TBD** (dataset-specific citation to be added)
- https://openneuro.org/datasets/ds002080/versions/4.0.1
- Post-operative brain tumor case cohort including diffusion MRI (TE/TR, b-values, voxel size, and preprocessing steps should be read from dataset sidecars/derivatives).

### BTC pre-op (OpenNeuro ds001226)
- **TBD** (dataset-specific citation to be added)
- https://openneuro.org/datasets/ds001226/versions/5.0.1
- Pre-operative brain tumor diffusion MRI cohort (TE/TR, b-values, voxel size, and preprocessing steps should be read from dataset sidecars/derivatives).

## b-tensor encoding

### Cardiff dataset
- **TBD**
- **TBD**
- b-tensor encoded diffusion MRI acquisition (linear/planar/spherical encoding expected; full protocol parameters still to be confirmed).

### Kerkelä dataset
- Kerkelä, L., Henriques, R. N., Hall, M. G., & others. (2020). *Constrained and rotationally invariant mapping of microscopic diffusion anisotropy with diffusion-relaxation MRI*.
- **TBD**
- Tensor-valued diffusion encoding dataset for microstructure modeling (protocol details should include LTE/PTE/STE b-tensor schemes; exact table still to be filled).

## Multi-TE

### SciDB dataset
- **TBD**
- https://www.scidb.cn/en/detail?dataSetId=411f844eb7974da68d08569a1cb27693#p2
- Multi-echo diffusion MRI dataset; full protocol parameters (TE train, TR, b-values, voxel size) and preprocessing details still to be extracted.

## Time-varying gradients

### 300 mT/m gradient comprehensive dataset
- Jones, D. K., Alexander, D. C., Cercignani, M., et al. (2021). Comprehensive diffusion MRI dataset for in vivo human brain microstructure mapping using 300 mT/m gradients. *Figshare collection*.
- https://springernature.figshare.com/collections/Comprehensive_diffusion_MRI_dataset_for_in_vivo_human_brain_microstructure_mapping_using_300_mT_m_gradients/5315474
- High-gradient diffusion MRI (up to 300 mT/m) with broad protocol coverage for microstructure mapping; acquisition table includes multiple diffusion timings and b-value regimes, with accompanying preprocessing in released derivatives.
