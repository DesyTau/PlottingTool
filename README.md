# PlottingTool

The root macro Plot.C loop over all the (nested)(sub)TDirectories inside a root file which name is passed as argument (see xAlberto_wPUwLepSF_htt_mt.inputs-sm-13TeV-histos as example),when a directory with a TH1 inside is found the function plot_hist() plots the histograms found in the directory, then the macro will continue to loop over the other directories.
                                                                                                                   
WARNING: the directories with the TH1s have to be the most nested ones, i.e. with no other subdirectories (see the example file).        
                                                                                                                  
Auxiliary functions definitions are at the bottom

OUTPUT: the macro will create directories named "output_"+ /name of the directories with inside the variables 
subdirectories/ and then put the plots and the latex tables inside these directories. 
