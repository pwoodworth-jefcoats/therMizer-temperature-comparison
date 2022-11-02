# therMizer Regional Model Temperature Comparison
This respository is for our regional comparison of temperature sensitivities using the `therMizer` extension of `mizer`.  If you're intersted in contributing to the comparison, here's what you'll need to get started:  
* A calibrated `mizer` model for your region of interest  
  + Ideally this model has been published.  At this point, though, it’s fine if you’re still working on the initial publication for the model.  Please don’t let that stop you from contributing.  
* Temperature-related model parameters  
  + For each species, you’ll need a minimum and maximum thermal tolerance.  You can find this from tagging studies, in [Fishbase](https://www.fishbase.se/search.php), or infer it from depth and location of occurrence.  
* ISIMIP 3a forcing for your region  
  + Plankton densities for creating a dynamic background resource  
  + Fishing forcing  
  + Temperature(s) to which each species is exposed.  This can be vertically and horizontally averaged, allocated across depth strata to replicate diel vertical migration, whatever makes the most sense for your region and species.  
  
Once you have everything you need, you can use the [therMizer package](https://github.com/sizespectrum/therMizer) to run four simulations, all with plankton and fishing forcing included:  
* No temperature functions  
* Temperature applied to metabolism only  
* Temperature applied to aerobic scope only  
* Full inclusion of temperature functions  

My goal is for us to share code here.  More to come on that soon.  For now, you can use my [FishMIP GitHub repo](https://github.com/pwoodworth-jefcoats/therMizer-FishMIP-2022-HI) as a guide.  It has the code I’ve used to run the FishMIP simulations for my region of interest (the fishing grounds of Hawaii’s longline fisheries in the central North Pacific Ocean).  I’ve tried to comment it thoroughly so that others can use it as a guide, and questions and comments are always welcome.

Also to come: which data to share and how.

