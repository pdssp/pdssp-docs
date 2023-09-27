(pdssp_stac_model)=
# PDSSP STAC Model

## Catalog structure

The STAC model allows to define static hierarchical relationships within a catalog. Collections can be logically grouped into a catalog, which can be part of parent catalog and may have sub-catalogs.

The PDSSP STAC static catalog structure, and where the source collections lay within that structure, can be defined as a Registry YAML file hosted on a GiHub repository (see [](pdssp_registry_ug)).

```{note} Inventory of [PDSSP Data Collections](https://docs.google.com/spreadsheets/d/1qTXSxcM2fxoUs_MuEs0AOE4QxvzfCDgfgfhTeCDmUuc/edit?usp=sharing) (Google Sheet){{ external_link }}.
```

Options considered for the catalog structure:

- Flat structure
- By target body only
    - Provides an overview of the metacatalog content, although this could be provided by a “target body” dynamic classification collection.
        - However, this dynamic collection by target references data products, not collection.
            - Both could be complementary
        - A collection can be primarily related to a target body, but a fraction of the data products within that collection might relate to other target bodies. For example, the OMEGA EDR collection mainly relates to Mars but also contain data about Phobos.
- By target body and data provider
    - This might be interesting for data providers (PDSSP labs) to quickly locate “their” data.
    - Alternatively, “data provider” could be use within the dynamic classification.

For example:

- PDSSP catalog
    - Mars catalog
        - PDS ODE Mars Data Products
            - MEX OMEGA EDR collection
            - MRO HIRISE EDR collection
            - MRO HIRISE RDRV11 collection
            - …
        - IAS/IDOC MEX OMEGA DDR collection (OMEGA_C_channel_Proj)
        - IAS/IDOC Mars Mineralogical Maps collection
        - IAS/IDOC Mars Features Catalog
            - Hydrated mineral sites
            - Central peaks hydrated phases between isidis and hellas
            - Seasonal South polar cap limits
            - …
        - IAS/IDOC MOCCAS Catalog
            - …
        - FU/Berlin Mars
            - HRSC hrsc3nd collection
            - ..
    - Titan catalog
        - VIM
    - Moon
    

## STAC Metadata

STAC collection/item metadata

```{note} Inventory of [PDSSP Data Models](https://docs.google.com/spreadsheets/d/1pLIS8iGU0IQ_LmgxtztdFTnT6D5L6-pk3-PKZdAYdWM/edit?usp=sharing) (Google Sheet){{ external_link }}.
```