# Probe-Recoverable Path Memory: Full Processed Data Package

This package consolidates the processed data products used for the current preprint evidence stack:

1. `01_ctmc_synthetic_validation/` — direct four-state CTMC witness for the framework.
2. `02_ground_truth_fret_benchmark/` — LabPresse/NatComm FRET benchmark trajectory-level validation with observed and ground-truth HDF5 traces.
3. `03_smfret_burst_benchmark/` — public Photon-HDF5 smFRET burst QC and latent mixture module.
4. `04_myosin5b_motor_pilot/` — myosin-5B public motor trajectory QC and local-step memory pilot.
5. `05_riboswitch_aggregate_module/` — riboswitch aggregate macrostate-insufficiency analysis from DG16/DG18 workbooks.
6. `06_tables_for_preprint/` — evidence hierarchy and preprint-facing summary tables.
7. `07_source_manifests/` — inclusion/exclusion record for raw sources.

## Central framework object

Probe-recoverable path memory tests whether preparation/history information is absent from the observed present but recoverable from later response:

    I(D;Y_T) = 0, but I(D;Z | Y_T) > 0.

The package is organized to avoid overclaiming. Only the CTMC and ground-truth FRET benchmark modules are direct trajectory-level framework validations. Public biological datasets are application-base modules showing latent structure, trajectory-pipeline behavior, or macrostate insufficiency.

## Critical interpretation boundaries

- CTMC module: positive direct synthetic witness.
- LabPresse FRET benchmark: positive ground-truth trajectory-level estimator validation, not empirical biological proof.
- smFRET burst benchmark: latent mixture/coarse observation validation, not path-memory proof.
- Myosin-5B: motor-side QC with an underpowered/negative conditional-memory result.
- Riboswitch aggregates: macrostate insufficiency at condition level, not individual-trajectory path memory.

## Raw source data

Large raw source archives are not duplicated here to keep the package portable. Processed outputs and small reproducibility-critical source files are included. See `07_source_manifests/source_file_inclusion_manifest.csv`.

## Recommended package citation/usage

Use this package as the processed-data and reproducibility companion for the framework preprint. For external datasets, cite the original dataset/article records in addition to this processed package.
