# SounDFi
SounDFi - Filter and detect erroneous data from a single echo-sounder 
 records.


#Downloading the software
  You can download the software either at:
    http://users.auth.gr/nezos/#Software
    
    or from the github.com
    
    https://github.com/stavkamp/SounDFi/
    


#Installing the software

  System Requirements 
  Operating System:       MS Windows 7 / MS Windows 10
  Free hard-disk space:   at least 2MiB
  .NET Framework:         v4.6.1 or newer

#Input Data Format
  #6 collumns, no headers, tab-delimited, depth values positive
  Identification Time Easting Northing EllipsoidalHeight Depth
ex:176 75346 480743.303  4439096.477  40.5489  1.296 

#Program parameters
  Sample size: Controls the sample size for the regression. It should 
    be a positive value and greater than the selected polynomial degree 
    plus one.
  Minimum possible measured depth: If a depth measurement is below this 
    positive value, it will be removed before the evaluation process.
  Maximum sampling distance: Sampling of values will stop once the 
    distance between the first and the last value exceeds this maximum 
    distance.
  Polynomial degree: Control the polynomial that will be regressed. The 
    lower the degree, the stricter the filter.
  Validation index threshold: If the index scoring factor is lower than 
    this percentage, then it will be classified as a possibleoutlier. 
    The closer to 100% the stricter the filter.  
   
 #Program outputs
   xx-Summary.txt
   xx-LessThanMinDepth.txt
   xx-Suspicious.txt
   xx-NotChecked.txt
   xx-Valid.txt
 
 
 #References
 
 #You can find a publication about the program here:
 
 https://www.psdatm.gr/index.php/latest-nes/2016-08-10-14-05-49/481-241 
 
  Please consider citing the software using the following reference:
  
      Kampourakis S, Bantola D-M (2018) Evaluation of global
    bathymetry models, coastlines and gravity reductions with
    data obtained from a hydrographic survey in Neos Marmaras
    in Chalkidiki. Department of Geodesy & Surveying, School of
    Rural and Surveying Engineering, Aristotle University of
    Thessaloniki (In Greek).
