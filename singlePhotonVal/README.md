simple validation of single photon samples
------------------------------------------

checks of
- number of PFOs
- energy response vs theta, phi, etc
- energy resolution
----------------------

go to the scripts directory
> cd ../scripts

edit the file validatePhoton.xml :
- specify the input files you want 
[you can mix different energies]
- specify the ROOT output filename you want

run it:
> Marlin  validatePhoton.xml

this should create a root file with lots of histograms

to visualise some useful plots, use the makePlots.py python script.
edit it with the input root file name (the one just produced in the previous step)

> export PYTHONPATH=${ROOTSYS}/lib
> python  makePlots.py

should produce a postscript (.ps) file with relevant plots.

questions/comments to
daniel dot jeans at kek dot jp

Dec.18, 2017