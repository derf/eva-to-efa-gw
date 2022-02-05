eva to efa gateway
---

This repository contains a EVA ID to EFA departure data helper for
[DBF](https://dbf.finalrewind.org). The **efa-gw** web service receives an EVA
stop ID originating from DB IRIS / HAFAS as input and returns [VRR
EFA](https://efa.vrr.de) departure data for the corresponding EFA stop. To do
so, it must map EVA IDs to EFA names or stopIDs. The translation table is
located in **share/vrr.json** and can be updated by feeding
[Haltestellen VRR](https://www.opendata-oepnv.de/ht/de/organisation/verkehrsverbuende/vrr/startseite?tx_vrrkit_view%5Bdataset_name%5D=haltestellen-vrr&tx_vrrkit_view%5Baction%5D=details&tx_vrrkit_view%5Bcontroller%5D=View)
and [IRIS stations.json](https://git.finalrewind.org/Travel-Status-DE-IRIS/plain/share/stations.json)
into **merge-haltestellen-and-iris**.

**share/vrr.json** is © DB Station&Service AG and Verkehrsverbund Rhein-Ruhr
AöR. It is licensed under the terms of [CC-BY
4.0](https://creativecommons.org/licenses/by/4.0/).
