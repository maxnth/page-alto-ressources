# page-alto-ressources
Resources for testing conversion from PAGE XML to ALTO

```
.
├── ...
├── origin                                          # Input files
│   ├── <Name>               
│         ├── basic.xml                             # Unaltered PAGE XML file
│         ├── extra_regions.xml                     # basic.xml + added extra regions (especially "uncommon" types)
│         ├── extra_text_style.xml                  # basic.xml + added text stlye optione (fontColour, …)
│         ├── destroyed_reading_order.xml           # basic.xml with altered/"destroyed" reading order
│         └── ...                                   # etc.
│  
├── output                                          # Converted output
│   ├── <Name>
│         ├── <JPageConverter>                      # Contained files were converted with "original" JPageConverter from Prima
│               ├── basic.xml                     
│               ├── extra_regions.xml             
│               ├── extra_text_style.xml          
│               ├── destroyed_reading_order.xml   
│               └── ...                           
│         ├── <AlteredPageConverter>                # Contained files were converted using a tweaked version of JPageConverter
│               ├── basic.xml                     
│               ├── extra_regions.xml             
│               ├── extra_text_style.xml          
│               ├── destroyed_reading_order.xml   
│               ├── extra_regions_advancedTags.xml  # Converted using a branch with more "advanced" Layout/… tagging
│               └── ...                             # etc.
└── ...
```
