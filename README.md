# MMM-swisstransport
Additional Module for MagicMirror²  https://github.com/MichMich/MagicMirror/tree/v2-beta

# Module: SwissTransport
This module displays traindepartures from your favourit trainstation.

## Using the module

To use this module, add it to the modules array in the `config/config.js` file:
````javascript
modules: [
    {
		module: 'MMM-swisstransport2',
		position: 'bottom_left',
		header: 'Zugverbindungen',
		config: {
			id: '008503203', // Trainstation ID
			maximumEntries: '10' // Max departures displayed
		}
	},
]
````
To find your Trainstation ID use http://transport.opendata.ch/v1/locations?query=Basel%20SBB
Replace query=...... with your stationname.


## Base API

This Modul is using the opendataCH/Transport API https://github.com/OpendataCH/Transport as apiBase
