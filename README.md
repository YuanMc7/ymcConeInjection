# ymcConeInjection
Fixed the bug where particles can not enter after restarting the computation using the ConeInjection model in OpenFOAM.com

The injection model has been tested in OpenFOAM-v2212

Usage:


1. Compile:

   wclean

   wmake


2. Add in controlDict:

   libs
   (
       "libmyConeInjection.so"
   );


3. Modify in sprayCloudProperties/subModels/injectionModels/:

   Injectors
   {
       type        myConeInjection;
       ................
   }

