# Datasets

## CAISO OASIS

CAISO datasets were sourced from:
* http://www.caiso.com
* http://oasis.caiso.com

CAISO datasets are described here:
* [CAISO OASIS Interface Specification](./caiso/OASIS-InterfaceSpecification_v5_1_8Clean_Independent2019Release.pdf)
    * Describes the available data feeds (called reports) and what the fields mean.
    * Each CAISO OASIS report is prefixed by 'data-oasis-' here
    * A report named FOO_BAZ_BAR would be named 'data-oasis-foo-baz-bar' here

However, the Interface Specification is pretty terse. See more CAISO documents
in this directory for the necessary context:

[CAISO Docs](./caiso)


### Available Datasets

There are 86 discrete databases listed here, and another 5 CAISO oasis
databases that are coming online shortly.

Note: some datasets have multiple databases listed here, as {00, 01, 02}.db.gz.
This is due to changes in the data feed xml schema over time, and is not
something that I've addressed yet. What this means is that for the first
schema, the database will be named `foo-bar-bing_00.db.gz`. That's typically
the one you want. however, if the schema changed at some point in time such
that subsequent inserts started to fail, then a second database would have been
created, leading to names like `foo-bar-bing_01.db.gz`.

If this affects you then please file an issue on github and we can address this
when it comes up.

* [data-oasis-ene-cb-mkt-sum](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-cb-mkt-sum/db/data-oasis-ene-cb-mkt-sum_00.db.gz)
* [data-oasis-prc-cd-intvl-lmp](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-cd-intvl-lmp/db/data-oasis-prc-cd-intvl-lmp_00.db.gz)
* [data-oasis-prc-nomogram-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-nomogram-dam/db/data-oasis-prc-nomogram-dam_00.db.gz)
* [data-oasis-prc-mpm-ref-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-mpm-ref-dam/db/data-oasis-prc-mpm-ref-dam_00.db.gz)
* [data-oasis-prc-mpm-cnstr-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-mpm-cnstr-dam/db/data-oasis-prc-mpm-cnstr-dam_00.db.gz)
* [data-oasis-prc-rtm-flowgate-rtm](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-rtm-flowgate-rtm/db/data-oasis-prc-rtm-flowgate-rtm_00.db.gz)
* [data-oasis-atl-peak-on-off](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-peak-on-off/db/data-oasis-atl-peak-on-off_00.db.gz)
* [data-oasis-prc-mpm-rtm-nomogram-cmp-hasp](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-mpm-rtm-nomogram-cmp-hasp/db/data-oasis-prc-mpm-rtm-nomogram-cmp-hasp_00.db.gz)
* [data-oasis-cbd-nodal-grp-cnstr-prc](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-cbd-nodal-grp-cnstr-prc/db/data-oasis-cbd-nodal-grp-cnstr-prc_00.db.gz)
* [data-oasis-atl-cbnode](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-cbnode/db/data-oasis-atl-cbnode_00.db.gz)
* [data-oasis-prc-cd-sptie-lmp](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-cd-sptie-lmp/db/data-oasis-prc-cd-sptie-lmp_00.db.gz)
* [data-oasis-ene-eim-dyn-nsi-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-eim-dyn-nsi-all-all/db/data-oasis-ene-eim-dyn-nsi-all-all_00.db.gz)
* [data-oasis-prc-eim-gh-rtd](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-eim-gh-rtd/db/data-oasis-prc-eim-gh-rtd_00.db.gz)
* [data-oasis-ene-cd-slrs-rtm](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-cd-slrs-rtm/db/data-oasis-ene-cd-slrs-rtm_00.db.gz)
* [data-oasis-atl-tiepoint](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-tiepoint/db/data-oasis-atl-tiepoint_00.db.gz)
* [data-oasis-atl-tiepoint](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-tiepoint/db/data-oasis-atl-tiepoint_01.db.gz)
* [data-oasis-atl-lap-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-lap-all/db/data-oasis-atl-lap-all_00.db.gz)
* [data-oasis-ene-eim-transfer-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-eim-transfer-all-all/db/data-oasis-ene-eim-transfer-all-all_00.db.gz)
* [data-oasis-atl-sp](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-sp/db/data-oasis-atl-sp_00.db.gz)
* [data-oasis-atl-sp](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-sp/db/data-oasis-atl-sp_01.db.gz)
* [data-oasis-sld-fcst-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-sld-fcst-dam/db/data-oasis-sld-fcst-dam_00.db.gz)
* [data-oasis-prc-dam-sch-cnstr-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-dam-sch-cnstr-dam/db/data-oasis-prc-dam-sch-cnstr-dam_00.db.gz)
* [data-oasis-ene-loss-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-loss-dam/db/data-oasis-ene-loss-dam_00.db.gz)
* [data-oasis-prc-mpm-rtm-nomogram-hasp](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-mpm-rtm-nomogram-hasp/db/data-oasis-prc-mpm-rtm-nomogram-hasp_00.db.gz)
* [data-oasis-atl-apnode-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-apnode-all/db/data-oasis-atl-apnode-all_00.db.gz)
* [data-oasis-prc-mpm-rtm-lmp-hasp-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-mpm-rtm-lmp-hasp-all/db/data-oasis-prc-mpm-rtm-lmp-hasp-all_00.db.gz)
* [data-oasis-prc-cd-rtm-nomogram-rctm-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-cd-rtm-nomogram-rctm-all/db/data-oasis-prc-cd-rtm-nomogram-rctm-all_00.db.gz)
* [data-oasis-prc-mpm-default-cmp-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-mpm-default-cmp-dam/db/data-oasis-prc-mpm-default-cmp-dam_00.db.gz)
* [data-oasis-as-mileage-calc-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-as-mileage-calc-all/db/data-oasis-as-mileage-calc-all_00.db.gz)
* [data-oasis-atl-sp-tie](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-sp-tie/db/data-oasis-atl-sp-tie_01.db.gz)
* [data-oasis-atl-sp-tie](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-sp-tie/db/data-oasis-atl-sp-tie_00.db.gz)
* [data-oasis-ene-eim-transfer-tie-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-eim-transfer-tie-all-all/db/data-oasis-ene-eim-transfer-tie-all-all_01.db.gz)
* [data-oasis-ene-eim-transfer-tie-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-eim-transfer-tie-all-all/db/data-oasis-ene-eim-transfer-tie-all-all_00.db.gz)
* [data-oasis-atl-ruc-zone-map](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-ruc-zone-map/db/data-oasis-atl-ruc-zone-map_00.db.gz)
* [data-oasis-sld-sf-eval-dmd-fcst](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-sld-sf-eval-dmd-fcst/db/data-oasis-sld-sf-eval-dmd-fcst_00.db.gz)
* [data-oasis-sld-sf-eval-dmd-fcst](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-sld-sf-eval-dmd-fcst/db/data-oasis-sld-sf-eval-dmd-fcst_01.db.gz)
* [data-oasis-as-req-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-as-req-dam/db/data-oasis-as-req-dam_00.db.gz)
* [data-oasis-atl-hub](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-hub/db/data-oasis-atl-hub_00.db.gz)
* [data-oasis-prc-rtm-nomogram-rtm](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-rtm-nomogram-rtm/db/data-oasis-prc-rtm-nomogram-rtm_00.db.gz)
* [data-oasis-prc-mpm-nomogram-cmp-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-mpm-nomogram-cmp-dam/db/data-oasis-prc-mpm-nomogram-cmp-dam_00.db.gz)
* [data-oasis-prc-curr-lmp-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-curr-lmp-all/db/data-oasis-prc-curr-lmp-all_00.db.gz)
* [data-oasis-atl-ti-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-ti-all-all/db/data-oasis-atl-ti-all-all_01.db.gz)
* [data-oasis-atl-ti-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-ti-all-all/db/data-oasis-atl-ti-all-all_00.db.gz)
* [data-oasis-atl-pub-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-pub-dam/db/data-oasis-atl-pub-dam_00.db.gz)
* [data-oasis-cmmt-ra-mlc-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-cmmt-ra-mlc-dam/db/data-oasis-cmmt-ra-mlc-dam_00.db.gz)
* [data-oasis-prc-mpm-rtm-ref-bus-hasp](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-mpm-rtm-ref-bus-hasp/db/data-oasis-prc-mpm-rtm-ref-bus-hasp_00.db.gz)
* [data-oasis-prc-rtm-lap](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-rtm-lap/db/data-oasis-prc-rtm-lap_00.db.gz)
* [data-oasis-ene-hrly-base-loss-dam-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-hrly-base-loss-dam-all/db/data-oasis-ene-hrly-base-loss-dam-all_00.db.gz)
* [data-oasis-sld-fcst-peak](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-sld-fcst-peak/db/data-oasis-sld-fcst-peak_00.db.gz)
* [data-oasis-atl-pub-sched](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-pub-sched/db/data-oasis-atl-pub-sched_00.db.gz)
* [data-oasis-ene-mpm-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-mpm-dam/db/data-oasis-ene-mpm-dam_00.db.gz)
* [data-oasis-sld-ren-fcst-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-sld-ren-fcst-dam/db/data-oasis-sld-ren-fcst-dam_00.db.gz)
* [data-oasis-crr-clearing-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-crr-clearing-all-all/db/data-oasis-crr-clearing-all-all_00.db.gz)
* [data-oasis-prc-hasp-lmp](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-hasp-lmp/db/data-oasis-prc-hasp-lmp_00.db.gz)
* [data-oasis-prc-fuel-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-fuel-all/db/data-oasis-prc-fuel-all_00.db.gz)
* [data-oasis-ene-aggr-flex-ramp-rtd](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-aggr-flex-ramp-rtd/db/data-oasis-ene-aggr-flex-ramp-rtd_01.db.gz)
* [data-oasis-ene-aggr-flex-ramp-rtd](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-aggr-flex-ramp-rtd/db/data-oasis-ene-aggr-flex-ramp-rtd_00.db.gz)
* [data-oasis-sld-adv-fcst-rtd](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-sld-adv-fcst-rtd/db/data-oasis-sld-adv-fcst-rtd_01.db.gz)
* [data-oasis-sld-adv-fcst-rtd](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-sld-adv-fcst-rtd/db/data-oasis-sld-adv-fcst-rtd_00.db.gz)
* [data-oasis-prc-mpm-rtm-flowgate-hasp-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-mpm-rtm-flowgate-hasp-all/db/data-oasis-prc-mpm-rtm-flowgate-hasp-all_00.db.gz)
* [data-oasis-trns-atc-dam-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-trns-atc-dam-all/db/data-oasis-trns-atc-dam-all_00.db.gz)
* [data-oasis-atl-baa-tie](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-baa-tie/db/data-oasis-atl-baa-tie_01.db.gz)
* [data-oasis-atl-baa-tie](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-baa-tie/db/data-oasis-atl-baa-tie_00.db.gz)
* [data-oasis-ene-eim-transfer-limit-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-eim-transfer-limit-all-all/db/data-oasis-ene-eim-transfer-limit-all-all_00.db.gz)
* [data-oasis-trns-usage-dam-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-trns-usage-dam-all-all/db/data-oasis-trns-usage-dam-all-all_00.db.gz)
* [data-oasis-trns-usage-dam-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-trns-usage-dam-all-all/db/data-oasis-trns-usage-dam-all-all_03.db.gz)
* [data-oasis-trns-usage-dam-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-trns-usage-dam-all-all/db/data-oasis-trns-usage-dam-all-all_05.db.gz)
* [data-oasis-trns-usage-dam-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-trns-usage-dam-all-all/db/data-oasis-trns-usage-dam-all-all_01.db.gz)
* [data-oasis-trns-usage-dam-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-trns-usage-dam-all-all/db/data-oasis-trns-usage-dam-all-all_02.db.gz)
* [data-oasis-trns-usage-dam-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-trns-usage-dam-all-all/db/data-oasis-trns-usage-dam-all-all_04.db.gz)
* [data-oasis-atl-itc-sp](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-itc-sp/db/data-oasis-atl-itc-sp_00.db.gz)
* [data-oasis-atl-gen-cap-lst](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-gen-cap-lst/db/data-oasis-atl-gen-cap-lst_01.db.gz)
* [data-oasis-atl-gen-cap-lst](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-gen-cap-lst/db/data-oasis-atl-gen-cap-lst_00.db.gz)
* [data-oasis-prc-curr-hub-lmp](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-curr-hub-lmp/db/data-oasis-prc-curr-hub-lmp_00.db.gz)
* [data-oasis-ene-eim-flex-ramp-input-rtm](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-eim-flex-ramp-input-rtm/db/data-oasis-ene-eim-flex-ramp-input-rtm_00.db.gz)
* [data-oasis-prc-mpm-nomogram-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-mpm-nomogram-dam/db/data-oasis-prc-mpm-nomogram-dam_00.db.gz)
* [data-oasis-ene-eim-transfer-limits-tie-rtd-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-eim-transfer-limits-tie-rtd-all/db/data-oasis-ene-eim-transfer-limits-tie-rtd-all_00.db.gz)
* [data-oasis-prc-ds-ref](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-ds-ref/db/data-oasis-prc-ds-ref_00.db.gz)
* [data-oasis-ene-disp](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-disp/db/data-oasis-ene-disp_00.db.gz)
* [data-oasis-ene-ea-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-ea-all-all/db/data-oasis-ene-ea-all-all_00.db.gz)
* [data-oasis-trns-curr-usage-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-trns-curr-usage-all-all/db/data-oasis-trns-curr-usage-all-all_00.db.gz)
* [data-oasis-prc-flex-ramp-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-flex-ramp-dam/db/data-oasis-prc-flex-ramp-dam_00.db.gz)
* [data-oasis-prc-mpm-cnstr-cmp-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-mpm-cnstr-cmp-dam/db/data-oasis-prc-mpm-cnstr-cmp-dam_00.db.gz)
* [data-oasis-prc-intvl-as-rtm](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-intvl-as-rtm/db/data-oasis-prc-intvl-as-rtm_00.db.gz)
* [data-oasis-ene-baa-mkt-events-rtd-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-baa-mkt-events-rtd-all/db/data-oasis-ene-baa-mkt-events-rtd-all_00.db.gz)
* [data-oasis-prc-ghg-allowance](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-ghg-allowance/db/data-oasis-prc-ghg-allowance_00.db.gz)
* [data-oasis-prc-cnstr-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-cnstr-dam/db/data-oasis-prc-cnstr-dam_00.db.gz)
* [data-oasis-ene-base-nsi-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-base-nsi-dam/db/data-oasis-ene-base-nsi-dam_00.db.gz)
* [data-oasis-as-results-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-as-results-dam/db/data-oasis-as-results-dam_00.db.gz)
* [data-oasis-ene-uncertainty-mv-rtd](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-uncertainty-mv-rtd/db/data-oasis-ene-uncertainty-mv-rtd_00.db.gz)
* [data-oasis-atl-tac-area-map](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-tac-area-map/db/data-oasis-atl-tac-area-map_00.db.gz)
* [data-oasis-trns-outage-all-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-trns-outage-all-all/db/data-oasis-trns-outage-all-all_00.db.gz)
* [data-oasis-cmmt-rmr-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-cmmt-rmr-dam/db/data-oasis-cmmt-rmr-dam_00.db.gz)
* [data-oasis-ene-wind-solar-summary](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-wind-solar-summary/db/data-oasis-ene-wind-solar-summary_00.db.gz)
* [data-oasis-as-op-rsrv](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-as-op-rsrv/db/data-oasis-as-op-rsrv_00.db.gz)
* [data-oasis-sld-fcst-actual](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-sld-fcst-actual/db/data-oasis-sld-fcst-actual_00.db.gz)
* [data-oasis-prc-cd-rtm-flowgate-rtm](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-cd-rtm-flowgate-rtm/db/data-oasis-prc-cd-rtm-flowgate-rtm_00.db.gz)
* [data-oasis-atl-osm-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-osm-all/db/data-oasis-atl-osm-all_00.db.gz)
* [data-oasis-atl-osm-all](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-atl-osm-all/db/data-oasis-atl-osm-all_01.db.gz)
* [data-oasis-prc-mpm-lmp-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-mpm-lmp-dam/db/data-oasis-prc-mpm-lmp-dam_00.db.gz)
* [data-oasis-ene-slrs-dam](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-ene-slrs-dam/db/data-oasis-ene-slrs-dam_00.db.gz)
* [data-oasis-prc-rtpd-lmp](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-prc-rtpd-lmp/db/data-oasis-prc-rtpd-lmp_00.db.gz)

## Content.Oasis

* [data-oasis-daily-renewables-output](https://s3.us-west-1.wasabisys.com/eap/energy-dashboard/data/data-oasis-daily-renewables-output/db/data-oasis-daily-renewables-output_00.db.gz)
