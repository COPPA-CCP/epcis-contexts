# EPCIS Contexts

Additonal contexts for EPCIS in the COPPA ecosystem based on [EPCIS](https://ref.gs1.org/standards/epcis/) and the [GS1 vocabulary](https://ref.gs1.org/standards/cbv/)

## Transporation Event

A transportation event is dedicated to map the transportation of a good in a single event, including all information neccessary to estimate the CO2 emission of the process.

[Example transport event](./examples/transport-event-single.jsonld)

Alternatively the transportation can be modelled with a series of shipping events.

Departure bizSteps: departing, shipping (summed up staging_unbound, loading und departing)
Arrival bizSteps: arriving, accepting, unloading

Checking for these events follows a destinct order

- accepting
- arriving
- unloading

- departing
- shipping
