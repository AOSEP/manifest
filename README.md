# ANDROID OPEN SOURCE EXTENDED PROJECT 
--------------------------------------

a custom Android firmware exclusively for supporting devices whose
OEM has been abandoned with latest software and security implementation.

# Credits
---------
* [**Nikhil C R**](https://www.linkedin.com/in/nikhil-c-r-9153b162)
* [**Neenu P A**](https://www.linkedin.com/in/neenu-p-a-291045b8)
* [**ANJALI KRISHNAN**](https://www.linkedin.com/in/nikhil-c-r-9153b162)


# How to Build?
-------------

To initialize your local repository using the AOSEP trees, use a 
command like this:

```bash
  repo init -u git://github.com/aosep/manifest.git -b 9.0
```
  
# Then to sync up:
----------------

```bash
  repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

# Finally to build:
-----------------

```bash
  . build/envsetup.sh
  lunch aosep_device_codename-userdebug
  mka aosep -j$(nproc --all)
  where j$ denotes the number of available cores
  ...

