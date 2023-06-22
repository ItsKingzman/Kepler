My project is based on the dataset from the Kepler Exoplanet Search. The Kepler Space Observatory is a NASA-build satellite that was launched in 2009. The telescope is dedicated to searching for exoplanets in star systems besides our own, with the ultimate goal of possibly finding other habitable planets besides our own. The original mission ended in 2013 due to mechanical failures, but the telescope has nevertheless been functional since 2014 on a "K2" extended mission.
Kepler had verified 1284 new exoplanets as of May 2016. As of October 2017, there are over 3000 confirmed exoplanets total (using all detection methods, including ground-based ones). On October 30, 2018, after the spacecraft ran out of fuel, NASA announced that the telescope would be retired. The telescope was shut down the same day, bringing an end to its nine-year service.

The problem I am trying to solve is if a planet is CONFIRMED, then what exactly makes it a planet? What attributes are required for that? What percentage of the planets are CONFIRMED, CANDIDATES or FALSE POSITIVES.

My data is pre-processed. Some of the important attributes of the data are: kepoi_name: A KOI (KEPLER OBJECT OF INTEREST) is a target identified by the Kepler Project that displays at least one transit-like sequence within Kepler time-series photometry that appears to be of astrophysical origin and initially consistent with a planetary transit hypothesis
kepler_name: [These names] are intended to clearly indicate a class of objects that have been confirmed or validated as planets—a step up from the planet candidate designation.
koi_disposition: The disposition in the literature towards this exoplanet candidate. One of CANDIDATE, FALSE POSITIVE, NOT DISPOSITIONED or CONFIRMED.
koi_pdisposition: The disposition Kepler data analysis has towards this exoplanet candidate. One of FALSE POSITIVE, NOT DISPOSITIONED, and CANDIDATE.
koi_score: A value between 0 and 1 that indicates the confidence in the KOI disposition. For CANDIDATEs, a higher value indicates more confidence in its disposition, while for FALSE POSITIVEs, a higher value indicates less confidence in that disposition.

I was able to clean my data and I have a deeper understanding of it as well. I was able to implement logistic regression as well as k-means clustering. I struggled a little with the plotting of certain things. The names of the attributes were a little confusing so I changed them into something more readable and got rid of the ones with NaN values. Figuring out the correlation matrix was very tough and took me about 2 days to implement. I also made a histogram expressing what spectral classes the stars are in. I also created a scatterplot that shows the stellar surface gravity (stellar_surf_gravity) vs. stellar radius (stellar_radius), depicting each star in its color. I had fun creating a 3D scatterplot that shows the Gravity vs. Temperature vs. Radius. 

For my final task, I was able to find planets that are habitable (Often called Goldilocks planets).
