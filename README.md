# Strava Tools - an ArcGIS Pro Python Toolbox!

**`Strava Tools`** is an ArcPy-based ToolBox for use in ArcGIS Pro 3.1! Right now, it comprises one tool: **`ImportActivityRoutes`**, which allows you to pull activity routes from the Strava API and convert them into an ArcGIS Pro Polyline feature class. I plan to work on more tools in the future, but this one is enough to get you started on cool projects of your own!

### Prerequisites

 1. A Strava API Account:
	 - This one sounds complicated, but I promise, it's not! Any Strava user can go to [https://www.strava.com/settings/api] to make generate a Client ID, Client Secret, Access Token, and Refresh Token. Simply copy those 4 items into the included `strava_api_auth_template.json` file. You'll include that file as an input to the `ImportActivityRoutes` tool.
 2. ArcPy Conda Environment with the `polyline` package
	 - This package is not included in the default `arcgispro-py3` environment, so you can easily fix that by going to "ArcGIS" -> "Python Command Prompt" and running `conda install -n arcgispro-py3 polyline`. You can also import it to a different environment, if desired.
	 - All other package dependencies should already exist in the default `arcgispro-py3` environment (`arcpy`, `json`, `requests`, `datetime`, `pandas`)

### Usage
It's easy! Copy the contents of the `source` folder here to a folder accessible via ArcGIS Pro. Open your ArcGIS Pro project, and in the Catalog pane, right click Toolboxes, and then select "Add Toolbox". 

Select `Strava_Tools.pyt` in the pop-up explorer. Now you should be good to go!
<img src="https://github.com/garretts-hub/Strava_Tools/blob/main/images/using_tool.png" alt="Using the Toolbox" title="Using the Toolbox">
Documentation for each tool parameter is provided in the "Help" icon when hovering over each input.
<img src="https://github.com/garretts-hub/Strava_Tools/blob/main/images/parameters.png" alt="Tool Parameters" title="Tool Parameters">
<img src="https://github.com/garretts-hub/Strava_Tools/blob/main/images/Logging.png" alt="Verbose Logging" title="ArcGIS Tool Messages">
<img src="https://github.com/garretts-hub/Strava_Tools/blob/main/images/output.png" alt="Output Feature Class" title="Output Feature Class">

#### Change Log
|Version|Date|Summary of Changes|
|--|--|--|
|v1.0|Sep. 17, 2023|Initial Project Publication|