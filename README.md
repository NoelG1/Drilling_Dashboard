# Drilling_Dashboard
This project was developed as part of a 1-day Hackathon organized by Seisware in Edmonton Alberta Canada. The focus was on automation in the field of geoscience. The project resulted in a win as "Audience Favorites". We developed a dashboard for directional drilling and seismic data, with a shareable link that can be displayed on any device. The idea was to eliminate the need to use a 3rd party software, like Petrel or Seisware, in order to view or share subsurface visuals.

Competition blog: [Seisware Blog](https://seisware.com/geoscience-hackathon2019/)

# Dataset
A 3D (public domain) seismic volume from New Zealand ([Parihaka](https://wiki.seg.org/wiki/Parihaka-3D)) was used, which includes a full angle stack, near, mid and far stacks.

*[Download Link](https://wiki.seg.org/wiki/Parihaka-3D#Download_data_clicking_links_or_command_line_wget)*
(**Note**: File is 4.7 GB)

# Script Breakdown
We used segyio to read in the segy file
```
import segyio as sg
```
and then for isolating inlines and crosslines a jupyter notebook widget was used, then plotly to display the dashboard.
