---
path: help-pages/vehicles
date: 2019-06-07T20:19:31.478Z
title: Transfer ELD Data File - Vehicles
---
# Transfer ELD Data File - Vehicles

## Topics in this section:

*   [What is the purpose of the "Transfer ELD Data File - Vehicles" page?](#A)
*   [Transferring ELD Data Files](#B)

## What is the purpose of the "Transfer ELD Data File - Vehicles" page?

The "Transfer ELD Data File - Vehicles" page is intended to allow carriers to electronically submit drivers' ELD records of duty status (aka [driver logs](https://app.qa.efleetsuite.com/eFleetSuite/Help/ViewLog.aspx)) to the [FMCSA](https://app.qa.efleetsuite.com/eFleetSuite/Help/Glossary.aspx) eRODS system. Electronic submittal is used when requested by an authorized safety official as required by _49 CFR 395.22 (j) Record Production_. The "Transfer ELD Data File - Vehicles" page is used when the authorized safety official requests driver logs corresponding to one or more vehicles over a date range.

## Transferring ELD Data Files

### To submit logs for one or more vehicles:

1.  Select the range of [dates](https://app.qa.efleetsuite.com/eFleetSuite/Help/FAQ_General.aspx#A.5) for which you wish to transfer logs.

    ##### To change a date:

    *   Click the **...** button to pop up the calendar.
    *   Click on the date desired.
2.  Choose the means used to submit the logs to the [FMCSA](https://app.qa.efleetsuite.com/eFleetSuite/Help/Glossary.aspx) (normally this will be as requested by the safety official).
    *   Select **Web Services** to transfer the logs using the FMCSA's Web Services submittal method.
    *   Select **Email** to transfer the logs using the FMCSA's email submittal method.

    #### * Note that secure encryption is used to transfer logs in both cases.

3.  Select the vehicles for which you wish to transfer logs.

    ##### To select vehicles:

    *   Click on a vehicle ID in the **Available Vehicles** list to highlight it.
    *   Click the **Add** button to add the vehicle to the **Selected Vehicles** list.
    *   If a vehicle is added in error, click the Vehicle ID in the **Selected Vehicles** list to highlight it, then click the **Remove** button.
    *   Repeat until the **Selected Vehicles** list contains the desired vehicles.
4.  Enter a file comment (optional). The safety official may specify a file comment to use.
5.  Click the **Submit log data to FMCSA** button.

This will initiate log transfer to the FMCSA for the selected vehicles and date range.

#### * Hold down the Ctrl key on your keyboard while clicking with your mouse in order to highlight multiple vehicles. When all desired vehicles are highlighted, release the Ctrl key and click the **Add** or **Remove** button as appropriate.

### Some things to consider when transferring ELD Data Files:

*   When the **Submit log data to FMCSA** is pressed and the web page refreshes, the system has queued the request internally. The system will continue working in the background to submit the driver logs to the FMCSA.
*   A single ELD Data File corresponds to driver logs for a specific driver and date range. When submitting logs for one or more vehicles, eFleetSuite determines which drivers used the selected vehicles, and on which dates, and submits corresponding driver logs for those dates. The driver logs may span a day before or after the usage of any particular vehicle. Also, the driver logs will include vehicle activity for the selected vehicles.
*   The FMCSA eRODS will receive one or more driver log submittals for each driver who operated any of the selected vehicles in the date range. If the selected date range covers more than 31 days, the submittals may be split on month boundaries.
*   Only drivers who have used an ELD are available for ELD Data Transfer. Drivers who have only ever used an AOBRD cannot have their logs electronically transferred to the FMCSA.
*   When the selected date range includes a driver's AOBRD use prior to first using an ELD, the earliest logs that will be transferred are limited to 7 days prior to first ELD use.
*   A vehicle that was equipped with only an AOBRD during part of the selected date range will only have ELD Data Files transfered if the vehicle was used by a driver who also used an ELD.
