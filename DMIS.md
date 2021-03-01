
# Overview
The Data Matching and Imputation System is maintained by GARFO. Just email Michael Lanning at GARFO, he's got all the answers. j.michael.lanning@noaa.gov 

Tables: 
APSD.t_ssb_trip@garfo_nefsc
APSD.t_ssb_catch@garfo_nefsc 
APSD.t_ssb_discard@garfo_nefsc

APSD.t_ssb_trip_current@garfo_nefsc
APSD.t_ssb_catch_current@garfo_nefsc 
APSD.t_ssb_discard_current@garfo_nefsc


Location: GARFO super secret server

Schema: 


# Linking to Veslog

Linking to VESLOG with DMIS DOCID has a few issues. (Chad Demarest, May 14, 2020)
1.  JML adds digits to DMIS DOCID to denote subtrips.
1.  Another is that some data handling protocols (varies by file type) truncate a digit off the end of the EVTR serial numbers.
1.  A third is that DMIS will Give positive (mostly correct) match’s where the DOCID fails for these and other reasons.



# On Home Consumption Fish

> The code for this stuff is BHC_ (either _LIVE_POUNDS or _LANDED_POUNDS).  "BHC" stands for "Bait and Home Consumption".  A few years ago they added LUMF (Legal UnMarketable Fish) to this category as well.  LUMF, at lease for here, and at least as I understand it, is derived from observer trips only.  But I'm not 100% sure on that. If you use DLR_LIVE or DLR_LANDED (or DLR_DOLLAR) you won't get the BHC fish.  If you use LANDED or POUNDS or DOLLAR_SSB/GDP you'll get 'em, plus imputed values for the DOLLAR field. Starting on the next run of DMIS, fish that are authorized to be landed on EFP trips but are not sold thu a dealer will be added to the BHC_ fish.   Chad's email April 11, 2018.

# Versions

> There is a "_current" versioning of tables. As of April 2020, current contains a little bit more data. I now use _trip for everything, whereas a yearly ago I used _current.  There were some discrepancies for earlier years (2013?) that _trip had correct and _trip_current did not.  Otherwise I believe they are the same. (Chad)

> I have been using current since there is more recent data included. Hopefully for older data the two match up, but I haven't looked into that in a while. (Greg)