# GeoNode
# by Felipe Oliveira
# March 2011
# [http://geeks.aretotally.in/projects/geonode] (http://geeks.aretotally.in/projects/geonode)
# [http://twitter.com/_felipera] (http://twitter.com/_felipera)

GeoNode adds very basic, but simple to use, geocoding capabilities to Node.js using Google's Geocode API - Geo Spatial is coming out soon.

## Usage

		var geonode = require('../lib/geonode');
		
		var address = '885 6th Ave #15D New York, NY 10001';
		var sensor = false;
		geonode.geocoder(geonode.google, address, sensor, function(formattedAddress, latitude, longitude) {
			console.log("Formatted Address: " + formattedAddress);
			console.log("Latitude: " + latitude);
			console.log("Longitude: " + longitude);
		});