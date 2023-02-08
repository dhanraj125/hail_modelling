# hail_modelling



In this project we are calculating hail risk for each postcode using hail data of last 100 years. Hail risk is calculated based on the hail size and the hail storm frequency.

Input data used for the project is shapefile for postcode in Australia and the data for hail size and hail frequency is got from Beaurou for Meteorology, Australia.

The workflow for the project is as follows

1.	From hail lat/lon location point shapefile is created
2.	Using postcode shapefile and point data of hail, number of hail events per postcode is calculated.
3.	Using number of hail events and its size average hail size percode is calculated.
4.	After the calculation of postcode area frequency per unit is calculated.
5.	Normalized hail size is calculated (between 0 and 1) using average hail size per postcode.
6.	Normalized hail frequency is calculated using frequency per unit area.
7.	hail risk is the average percentage of normalized hail size and normalized hail frequency per unit area.
