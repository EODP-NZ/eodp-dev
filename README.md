eodp-dev
========

#NZ Environmental Observations Data Profile - Developers repository

## Introduction

The EODP is a profile of WFS that allows the discovery of timeseries data associated with monitoring stations. This forms part of a larger project to enhance the interoperability of Environmental Observations throughout New Zealand.

Organisations such as NIWA, Landcare, GNS and Regional councils maintain a range of monitoring stations making environmental observations. These include Climate, Hydrology, Air Quality, Soils, Water Quality, and Marine data.

We wish to make this data available for research, analysis and reporting through open data protocols such as the Sensor Observation Service (SOS), Web Feature Service (WFS), Web Coverage Service (WCS) and Web Mapping Service (WMS). We also want to publish the existance of such data sets and services through online metadata catalogues (CSW).

In order to make use such data services users must first be able to discover their existence and then accurately select the subset of data that is relevant to their needs. The EOPD is focussed on this selection process in essence addressing the Where, What and When questions.

WFS provides a rich filtering capability: http://www.opengeospatial.org/standards/filter but typical WFS sources use a flat property/value schema that makes it difficult to express the many to one relationship of the timeseries measurements taken at a station. The EODP is an Application Schema for WFS that encodes the station metadata as a nesting of SF_SpatialSamplingFeature and OM_Observations using the language of Observations and Measurements to describe the characteristics of the timeseries.

The profile is extended by the use of an external Vocabulary service used to dereference measurement identifiers into familiar timeseries names such as rainfall or temperature.
