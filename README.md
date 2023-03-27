# IO-PrincipiaGravityModels
A set of configs to give axial tilt, for use in ***Principia***.

Most axial tilts were chosen arbitrarily. Many are designed to resemble their body's real-life analogues, but there exists varying degrees of faithfulness in their representations. In other cases, tidally locked-bodies were given axial tilts to match their orbits. 

Many of the values which were based off the bodies orbits (such as in tidally-locked bodies) were not based off stock orbits but rather those included in ***IO-AlteredOrbits***. These tilts are designed to be paired with such orbital changes. The stock orbits are so very plain and mostly in-line with the ecliptic that there exists little need for tilts in vanilla KSP.

Please note that as per ***Principia*** requirements (https://github.com/mockingbirdnest/Principia/wiki/Principia-configuration-files#the-principia_gravity_model-configuration) there must exist no more than one node (i.e. only one config file should not have an "@" symbol as its first character). As such, if the stock gravity model is not used (due to a planet pack replacement or similar) but another is, one of them must be made to be the root node. What that means is that if one is to not make such a change themself, or in any case where one of these config files are used, ***IO-PrincipiaGravityModel-Stock*** is a **dependancy**. It should be said that ***Principia*** is a dependancy in order for these configs to work, but it *should* not cause an error to have these installed but not ***Principia***.

In the same vein, please note that such systems that replace the stock Kerbin and/or Sun ("Kerbol") still (as far as I believe) use the names *Kerbin* and *Sun* internally to refer to the bodies that replace them. In this case, ***IO-PrincipiaGravityModel-Stock*** will conflict with such a mod, as it will (likely) provide incorrect/undesired axial tilt and gravitational parameter values.

If you wish to make your own gravity model, follow the format I have provided, the config included in ***Principia*** (***Principia/real_solar_system/gravity_model.cfg***), or the ***Principia*** wiki (https://github.com/mockingbirdnest/Principia/wiki/Principia-configuration-files#the-principia_gravity_model-configuration).


Lastly, while included, the config for ***GEP*** may or may not cause incorrect *reference_angle* (*initialRotation*) states for ***GEP*** bodies (which, if an issue, can be fixed by enabling the variable assignment and finding the correct phase shift). Such a case presented itself when making the ***Kcalbeloh*** config, wherein the phase shift was -90. ***Principia*** does not seem to note this issue, and believes 0 is the correct value for *reference_angle* to give an *initialRotation* of also 0. I believe this is only an issue in added star systems.

At the present moment I also have no intention to confirm this issue nor fix it, and I do not plan to maintain the configs for ***GEP (v1.2.8)*** or ***Kcalbeloh (v1.0.1)*** henceforth.
