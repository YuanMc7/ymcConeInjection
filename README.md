# ymcConeInjection
Fixed the bug where particles can not enter after restarting the computation using the ConeInjection model in OpenFOAM.com

The injection model has been tested in OpenFOAM-v2212

Usage:

In controlDict:

//-----------------------------------//
libs
(
    "libmyConeInjection.so"
);
//-----------------------------------//



In sprayCloudProperties/subModels/injectionModels/:

//-----------------------------------//
Injectors
{
    type       myConeInjection;
    ................
}
//-----------------------------------//

