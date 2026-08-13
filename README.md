# Awesome-Fleet-Electrification

## Top Fleet Electrification Platforms



A curated list of leading platforms for fleet electrification — covering EV suitability analysis, charge management, depot optimization, telematics integration, energy management, route planning for electric vehicles, and mixed-fleet operations.  

**Primary focus: open-source software.**



Commercial / hosted platforms are listed separately for completeness. Open-source alternatives and community tools are emphasized throughout.



---



## SaaS / Hosted Platforms



| Platform | Description | Key Focus |

|----------|-------------|-----------|

| **[Samsara](https://www.samsara.com/)** | Connected operations platform with dedicated fleet electrification tools for EV suitability analysis, charge control, mixed-fleet management, energy monitoring, and scaling zero-emission operations. | End-to-end fleet electrification + telematics |

| **[Geotab](https://www.geotab.com/)** | Leading telematics platform with strong EV and electrification planning capabilities, charging insights, and data-driven transition support for large mixed fleets. | Telematics-led electrification planning |

| **[ChargePoint Fleet](https://www.chargepoint.com/)** | Integrated fleet charging and management platform connecting vehicle data, charging hardware, energy management, and analytics for depot and on-route operations. | Fleet charging + energy management |

| **[AMPECO](https://www.ampeco.com/)** | White-label, API-first EV charging management system (CSMS) with fleet features, billing, energy management, and policy-driven managed charging. | Charge point management & fleet charging |

| **[Optibus](https://www.optibus.com/)** | Transit planning and scheduling platform with specialized support for electric bus fleets, depot charging constraints, vehicle/crew scheduling, and zero-emission operations. | Electric transit planning & scheduling |

| **[BetterFleet](https://www.betterfleet.com/)** (formerly EVenergi) | AI and digital-twin platform for mission-critical fleets to plan, procure, and operate zero-emission vehicles and charging infrastructure while optimizing cost and readiness. | Zero-emission fleet planning & operations |

| **[Hitachi ZeroCarbon](https://www.hitachi.com/)** | Fleet electrification and charging optimization solutions (including ZeroCarbon Charge) focused on live vehicle monitoring, load balancing, tariff optimization, and cost reduction. | Charging optimization & fleet monitoring |

| **[Optiwatt Fleet](https://optiwatt.com/)** | Energy management and managed-charging platform that optimizes EV charging as a distributed energy resource, with utility-scale programs and direct vehicle connections. | Managed charging & VPP-style energy control |

| **[Volteras](https://www.volteras.com/)** | Vehicle data platform providing OEM and fleet data streams (battery, charging status, etc.) that power electrification and charge-optimization solutions. | Vehicle data for electrification |

| **[EVenergi](https://www.evenergi.com/)** / BetterFleet | Planning, procurement, and operations software for zero-emission fleets and infrastructure (rebranded/related to BetterFleet). | EV fleet & infrastructure planning |



---



## Open-Source Softwares



Fully featured commercial-grade fleet electrification platforms (EV suitability engines, multi-depot optimization, deep OEM telematics, and utility-grade energy management) are limited in pure open source. Strong open-source foundations exist around the OCPP protocol, charge station management systems (CSMS), and related energy/telematics building blocks.



### Core Frameworks & Charging / Fleet Platforms



| Project | Description | License | Notes |

|---------|-------------|---------|-------|

| **[CitrineOS](https://github.com/citrineos)** (Linux Foundation Energy) | Open-source EV charge management backend supporting OCPP 2.0.1 and NEVI compliance. Enables provisioning, transactions, remote control, monitoring, and energy management. | Open source | Leading open CSMS foundation |

| **[OpenOCPP](https://openocpp.com/)** | Open-source embedded OCPP stack (1.6J and 2.0.1) for EV chargers — pre-certified path to interoperability and faster certification. | Open source | Charger-side OCPP implementation |

| **[OpenCPMS](https://www.opencpms.io/)** | Open-source Charge Point Management System for managing and controlling OCPP-connected charge points. Lightweight and scalable. | Open source | Open CSMS core |

| **OCPP CSMS projects** | Community implementations of OCPP 2.0.1 charging station management systems (microservices, WebSocket handling, transaction management). | Various | Extensible CSMS examples |

| **TopazEV / managed open CSMS** | Production-oriented platforms built on CitrineOS offered as open-as-a-service or self-hostable stacks. | Based on open source | Managed open charging backend |

| **General telematics & fleet open tools** | Open GPS/telematics collectors, device management, and fleet tracking projects that can be extended with EV-specific metrics (SoC, SoH, charging status). | Various | Telematics building blocks |



### Specialized Libraries & Related Tools



| Project | Description | Focus Area |

|---------|-------------|---------|

| **OCPP protocol libraries** | Open implementations and test tools for OCPP 1.6 / 2.0.1 / 2.1 message handling, security profiles, and device management. | Protocol compliance |

| **Energy management & load balancing** | Open algorithms and services for smart charging, peak shaving, tariff optimization, and depot load management. | Managed charging |

| **Routing & range optimization** | Open routing engines (OSRM, GraphHopper, Valhalla) extended with EV range, elevation, and charging-stop models. | EV route planning |

| **Battery & vehicle data models** | Open schemas and parsers for battery state-of-charge, state-of-health, and charging session data. | Vehicle telemetry |

| **Digital twin / simulation** | Open simulation frameworks for modeling depot charging, vehicle schedules, and energy demand. | Planning & what-if analysis |

| **Utility / DER integration** | Open interfaces and pilots for demand response, V2G, and virtual power plant (VPP) style control of fleet chargers. | Grid interaction |



### Additional Notable Open-Source Tools



- **Self-hosted CSMS stacks** — Deploy CitrineOS, OpenCPMS, or community OCPP CSMS projects to manage OCPP-compliant chargers without vendor lock-in.

- **Charger firmware & edge software** — OpenOCPP and related embedded stacks for manufacturers and operators building or customizing hardware.

- **Data pipelines** — Open collectors that ingest telematics and charger data into time-series databases for custom electrification dashboards.

- **Optimization solvers** — OR-Tools, PuLP, or custom optimizers for charging schedules, vehicle assignment, and energy cost minimization.

- **Visualization & analytics** — Grafana, Metabase, or custom dashboards for SoC monitoring, energy cost, and depot utilization.

- **Standards & interoperability** — Tools and test suites supporting OCPP, ISO 15118, and related e-mobility standards.



**Note:** Commercial platforms provide deep OEM integrations, proven EV suitability modeling, large-scale depot optimization, utility programs, and turnkey mixed-fleet operations. Open-source strength lies in standards-based charging management (OCPP/CSMS), which forms the critical backbone of any electrification stack. Full fleet electrification solutions typically combine open charging backends with commercial telematics, planning, or energy-management services.



---



## Quick Start Recommendations



| Goal | Recommended Starting Point |

|------|---------------------------|

| Open-source charge station management (CSMS) | **CitrineOS** or **OpenCPMS** |

| Embedded OCPP stack for chargers | **OpenOCPP** |

| Self-hosted / standards-based charging backend | CitrineOS-based or community OCPP CSMS projects |

| Full fleet electrification + telematics | **Samsara** or **Geotab** |

| Fleet charging hardware + software | **ChargePoint Fleet** |

| White-label / API-first CSMS | **AMPECO** |

| Electric transit & bus scheduling | **Optibus** |

| Zero-emission fleet planning & digital twins | **BetterFleet** (EVenergi) |

| Charging optimization & monitoring | **Hitachi ZeroCarbon** |

| Managed charging / energy programs | **Optiwatt** |

| Vehicle data for electrification apps | **Volteras** |



---



## Contributing



Contributions, corrections, and new open-source projects are welcome.  

Please open an issue or pull request.



---



**Last updated:** August 2026  

Emphasizing open-source tools while documenting the major commercial platforms for context. CitrineOS, OpenOCPP, and related OCPP/CSMS projects form the strongest open-source foundation for EV charging management; complete fleet electrification platforms remain predominantly commercial, especially for suitability analysis, depot optimization, and deep vehicle/OEM integrations.
