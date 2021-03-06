---
title: Aurora
description: Know when auroras might be visible at your location
ha_category:
  - Environment
ha_iot_class: Cloud Polling
ha_release: 0.39
ha_domain: aurora
---

The `aurora` platform uses the [NOAA Aurora Forecast](https://www.swpc.noaa.gov/products/aurora-30-minute-forecast) service to let you know if an aurora might be visible at your home location in the next 30 minutes, based off of current solar flare activity.

This service gives a number 0-100 representing the current likelihood of visible auroras at your latitude/longitude. By default this sensor is set up to trigger when the reported likelihood for your location is > 75. It updates every 5 minutes.

You can check the attributes of the sensor to see your exact forecast.

## Configuration

To add the aurora binary sensor to your installation, search for the Aurora integration through the Configuration -> Integrations menu.

Enter a name for your Aurora location as well as the longitude and latitude of the location (default to your Home Assistant location).

Click Submit to add the integration to your environment.

You can configure multiple locations by adding the integration multiple times.

## Options

Once installed you can adjust the threshold for this location by clicking on the Options link on the integration.

## Sensors

The integration will add a single binary sensor for each location you configure which will be in the state on when there is a forecast probability of Aurora viewing above your threshold and off when it is below your selected threshold.
