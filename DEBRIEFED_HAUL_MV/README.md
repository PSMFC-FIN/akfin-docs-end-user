
## NORPAC.DEBRIEFED_HAUL_MV

<!-- badges: start -->
<!-- badges: end -->

The NORPAC.DEBRIEFED_HAUL_MV is a snapshot of the NORPAC.DEBREIFED_HAUL
table provided daily by FMA.

This and other materialized views in AKFIN’s NORPAC schema refresh
nightly after the NORPAC load from FMA is complete.

### Base Data Sources

- [NORPAC.DEBREIFED_HAUL](https://www.fisheries.noaa.gov/inport/item/10659)
  provides haul level data from observer program.

This materialized view also merges in offload records from
NORPAC.DEBRIEFED_SPCOMP, NORPAC.DEBRIEFED_LENGTH, AND
NORPAC.DEBRIEFED_AGE when haul was unavailable as RECORD_TYPE =
‘OFFLOAD’ to facilitate an inner join within the Answers BI Repository.
These records are NULL for most fields.

### Ancilary data

- Vessel data from AKR.V_VESSEL or
- Deployment data (Deployment trip info and monitoring_status) from
  akr.MV_OBSERVED_DEPLOYMENT_TRIPS
- Haul and trip target info from akr.v_obs_haul
- Gear description from norpac.gear_type_codes or NORPAC.DOMESTIC_GEAR
- Gear performance from NORPAC.ATL_LOV_GEAR_PERFORMANCE
- FMP area and subarea from COUNCIL.FMP_AREA_V
- 

| COLUMN_NAME                         | COMMENTS |
|:------------------------------------|:---------|
| RECORD_TYPE                         | NA       |
| JOIN_KEY                            | NA       |
| T_TABLE                             | NA       |
| CRUISE                              | NA       |
| PERMIT                              | NA       |
| VESSEL                              | NA       |
| VESSEL_LENGTH                       | NA       |
| HAUL_SEQ                            | NA       |
| HAUL_JOIN                           | NA       |
| TRIP_SEQ                            | NA       |
| TRIP_JOIN                           | NA       |
| HAUL_DATE                           | NA       |
| HAUL                                | NA       |
| HAUL_PURPOSE_CODE                   | NA       |
| GEAR_TYPE                           | NA       |
| PERFORMANCE                         | NA       |
| VESSEL_TYPE                         | NA       |
| DEPLOYMENT_DATE                     | NA       |
| DEPLOY_LATITUDE                     | NA       |
| DEPLOY_LONGITUDE                    | NA       |
| DEPLOY_LONGITUDE_CONVERTED          | NA       |
| DEPLOY_LONGITUDE_SECONDS            | NA       |
| DEPLOY_LATITUDE_SECONDS             | NA       |
| DEPLOY_E_W                          | NA       |
| FISHING_DEPTH_FATHOMS               | NA       |
| BOTTOM_DEPTH_FATHOMS                | NA       |
| RETRIEVAL_DATE                      | NA       |
| DURATION_IN_MIN                     | NA       |
| LOCATION                            | NA       |
| RETRV_LATITUDE                      | NA       |
| RETRV_LONGITUDE                     | NA       |
| RETRV_LATITUDE_SECONDS              | NA       |
| RETRV_LONGITUDE_SECONDS             | NA       |
| RETRV_LONGITUDE_CONVERTED           | NA       |
| RETRV_E_W                           | NA       |
| GENERIC_AREA                        | NA       |
| NMFS_AREA                           | NA       |
| COBLZ_AREA                          | NA       |
| VESSEL_ESTIMATE                     | NA       |
| OFFICIAL_TOTAL_CATCH                | NA       |
| OBSERVER_ESTIMATE                   | NA       |
| OBSERVER_ESTIMATE_METHOD            | NA       |
| DENSITY                             | NA       |
| CATCHER_BOAT_ADFG                   | NA       |
| IFQ                                 | NA       |
| CDQ_CODE                            | NA       |
| SKATES_IN_SET                       | NA       |
| HOOKS_PER_SKATE                     | NA       |
| TOTAL_HOOK_POTS                     | NA       |
| HAUL_SAMPLED_BY                     | NA       |
| RANDOM_SAMPLE_TABLE                 | NA       |
| RANDOM_BREAK_TABLE                  | NA       |
| MM_PERCENT_MONITORED                | NA       |
| BIRD_DETERRENCE                     | NA       |
| BIRD_VERIFICATION                   | NA       |
| PROCESSOR                           | NA       |
| FISHING_START_DATE                  | NA       |
| DATE_OF_ENTRY                       | NA       |
| YEAR                                | NA       |
| LATDD_END                           | NA       |
| LONDD_END                           | NA       |
| LATDD_START                         | NA       |
| LONDD_START                         | NA       |
| SEABIRD_SAMPLE_TYPE                 | NA       |
| ATLAS_VERSION                       | NA       |
| AKFIN_LOAD_DATE                     | NA       |
| GEAR_DESCRIPTION                    | NA       |
| AK_GEAR                             | NA       |
| GEAR_PERFORMANCE_DESCRIPTION        | NA       |
| FMP_AREA                            | NA       |
| FMP_SUBAREA                         | NA       |
| FMP_GEAR                            | NA       |
| DEPLOYMENT_TRIP_PK                  | NA       |
| DEPLOYMENT_TRIP_START_DATE          | NA       |
| DEPLOYMENT_TRIP_END_DATE            | NA       |
| SAMPLING_STRATA                     | NA       |
| SAMPLING_STRATA_NAME                | NA       |
| SAMPLING_STRATA_DEPLOYMENT_CATEGORY | NA       |
| SAMPLING_STRATA_SELECTION_RATE      | NA       |
| MONITORING_STATUS                   | NA       |
| HAUL_TARGET_CODE                    | NA       |
| TRIP_TARGET_CODE                    | NA       |
| HAUL_TARGET_NAME                    | NA       |
| TRIP_TARGET_NAME                    | NA       |
| GEAR_MODIFIER_DESCRIPTION           | NA       |
| AKFIN_VDATE                         | NA       |
