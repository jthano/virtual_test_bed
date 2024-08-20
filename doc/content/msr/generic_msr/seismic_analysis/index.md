# Seismic Analysis Model

This model demonstrates the seismic analysis of a nuclear power plant (NPP) building that houses a reactor vessel and four steam generators. This model uses the [MASTODON](https://mooseframework.inl.gov/mastodon/index.html) application. This NPP building is a hypothetical molten-chloride fast reactor (NPP). Details of the NPP building are provided in [!citet](inl-ext-20-59608). This model is presented in two parts: (1) seismic analysis of just the foundation basemat on seismic isolators, and (2) seismic analysis of the full building on seismic isolators. The foundation basemat and the isolation system in both cases is identical. In each case, the modeling is briefly described and the results are presented. The mesh for both the parts of this model is generated in Cubit and the Cubit journal file (`fixed_base_with_isolators_new.jou`) for these meshes is also included in the folder of this model in the repository.

This model was adopted from the list of examples on the [MASTODON](https://mooseframework.inl.gov/mastodon/examples/index.html) website. For further information regarding [MASTODON](https://mooseframework.inl.gov/mastodon/index.html) please contact Dr. Bolisetti at chandrakanth.bolisetti@inl.gov.

!tag name=Seismic Analysis Model pairs=reactor_type:MSR
                       reactor:generic_msr
                       geometry:reactor_building
                       codes_used:MASTODON
                       computing_needs:HPC
                       fiscal_year:2021
                       sponsor:DOE_OTT
                       institution:INL
                       simulation_type:seismic_analysis

[Seismic Analysis Model - Part 1: Foundation Basemat Analysis](npp_building/npp_building_pt1.md)

[Seismic Analysis Model - Part 2: NPP Building Analysis](npp_building/npp_building_pt2.md)