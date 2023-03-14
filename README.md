![LabOverview](/Images/Lab.png)

# R3VIVAL - Repository of Room Responses and 360 Videos of a Variable Acoustics Lab

## SUMMARY OF THE DATA 
This datset contains Spatial Room Impulse Responses (SRIR) and 360 stereoscopic video recordings of a variable acoustics lab. The dataset contains:
- Spatial Room Impulse Responses (total of 272 SRIRs).
  - 30 source positions arranged in 3 concentric circles (1.5m, 2m, 3m) every 30 degrees. 
    - The largest circle contains only 6 positions due to room dimensions.
    - Directional sound source (Genelec 8320).
  - 4 source positions next to room corners.
    - Omnidirectional source (B&K 4295).
  - 1 receiver position (7 microphone open array from [^1]).
  - 8 acoustic panel configuration.
    - 5 uniform conditions (0%, 25%, 50%, 75%, 100% absorption).
    - 3 asymmetric configurations (right, right/back, right/back/left absorptive).
    
- Video captures
  - Stereoscopic 360 videos (resolution 4096 x 2160).
  - Captured with LivePlanetVR camera.
  - 2 rooms (Lab and RoomA - shoebox room).
  - 4 seconds duration.
  - Static scenes showing the empty room.
 
 <img src="/Images/Plan.png" alt="drawing" width="600"/>


## VARIABLE ACOUSTICS LAB
<img src="/Images/Lab0Abs.jpg" alt="drawing" width="250"/> <img src="/Images/Lab50Abs.jpg" alt="drawing" width="250"/> <img src="/Images/Lab100Abs.jpg" alt="drawing" width="250"/>

- Shoebox room
- Dimensions: 9.7 × 5.5 × 2.7 m (L × W × H) 
- RT60 at mid frequencies (500-1000 Hz) ranging from ~0.5 to 0.75 seconds.

<img src="/Images/T30.png" alt="drawing" width="600"/>


## Microphone array

- 7 Microphone array
  - Earthworks M50 (centre)
  - 6x DPA 4060
  - 10 cm diameter
 
<img src="/Images/FRLArray_10cmDiameter_pic.jpg" alt="drawing" width="300"/>

|    Channel	| Position     |	Azimuth	|    Elevation|  Microphone   |
| ----------- | ------------ | -------- | ----------- | -----------   |
|    1        |	Front        |	0       |	0           | DPA 4060      |
|    2        |	Back         |	180     |	0           | DPA 4060      |
|    3        |	Right Top    |	90      |	45          | DPA 4060      |
|    4        |	Left Top     |	90      |	45          | DPA 4060      |
|    5        |	Right Bottom |	270     |	-45         | DPA 4060      |
|    6        |	Left Bottom  |	270	    | -45         | DPA 4060      |
|    7        |	Center       |	N/A     |	N/A         | Earthworks M50 |


## 360 Stereoscopic Videos

![LabOverview](/Images/Lab.png)
![LabOverview](/Images/RoomA.png)

## How to use this data? (Work in Progress)

- Render Binaural Room Impulse Responses
  - Set up the Binaural SDM Toolbox and its dependencies[^2] 
  - Run the example file

- Generate video for a specific loudspeaker arrangement

- Combine the data with the Audiovisual Speech Corpus[^3] to generate synthetic multi-talker scenes. Note that the link on the original publication is no longer available. A mirror source is provided in[^4]

![LabOverview](/Images/OverlayExample.png)

## Contributing

See the [CONTRIBUTING](CONTRIBUTING.md) file for how to help out.


## License

R3VIVAL is CC-BY-4.0 licensed, as found in the [LICENSE](LICENSE) file.


## Contact

Sebastia V. Amengual (samengual@meta.com)

## References

[^1]: Amengual Garí, S. V., Arend, J. M., Calamia, P. T., & Robinson, P. W. (2021). Optimizations of the spatial decomposition method for binaural reproduction. Journal of the Audio Engineering Society, 68(12), 959-976. https://doi.org/10.17743/jaes.2020.0063
[^2]: https://github.com/facebookresearch/BinauralSDM/
[^3]: Kishline, L. R., Colburn, S. W., & Robinson, P. W. (2020). A multimedia speech corpus for audio visual research in virtual reality (L). The Journal of the Acoustical Society of America, 148(2), 492-495. https://doi.org/10.1121/10.0001670
[^4]: https://drive.google.com/drive/u/1/folders/1E_sC5SfjZCJOnkLkIN7MJ38-bwkAHQkY


