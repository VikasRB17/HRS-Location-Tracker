# HRS-Location-Tracker
This interactive python notebook shows how data from a hotel aggregator was verified for location accuracy since it is very important to show the right data to customers.

HRS is a famous hotel brokerage service for both private and corporate clients. When so many hotels are hosted on an aggregator's site, it is natural to rely on multiple sources to gather up-to-date information about their hotel partners. A concern that goes along with this is which of this data is trustworthy. In this notebook, the focus is on verifying that the location data for all hotels is accurate.

The approach used here is using 
1. OpenStreetMaps API
2. Google Maps API

We pass the Hotel name and street information to both APIs and parse the returned Latitude and Longitudes. Using these values, a diff is performed with the Lat-Long info saved in the HRS database.
