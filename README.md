# ymcConeInjection
Fixed the bug where particles can not enter after restarting the computation using the ConeInjection model in OpenFOAM.com

The injection model has been tested in OpenFOAM-v2212

Usage:


Compile:

     wclean

     wmake


Add in controlDict:

libs
(
    "libmyConeInjection.so"
);


Modify in sprayCloudProperties/subModels/injectionModels/:

Injectors
{
    type       myConeInjection;
    ................
}

