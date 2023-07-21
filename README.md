# SGLXMetaToCoords
SpikeGLX metadata readers

Code to read SpikeGLX metadata for a given binary, and create a geometry map for spike sorting or other analysis.
The output format is set in the code -- see the code comments for details.

This code uses the ~snsGeomMap, present in data taken with SpikeGLX 20230202-phase30 or later. For older data, it reads the ~snsShankMap, and has hardcoded physical dimensions for all Neuropixels probe part numbers. There is an option to create a new metadata file appending the ~snsGeometryMap.

# the agbondy fork adds a fourth output option (a matlab struct) but keeps the default the same. This has been submitted to Jennifer's repo as a PR so that's why the default behavior was preserved.
# this fork sets the default to option 4 (matlab struct) and is what we use in ks2jrc2.


