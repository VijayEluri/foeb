
## Build file(s) for the 'Freenet OSGi Experiment'
#### What this script can do:
 * gather all sources/prebuild libs
 * build, build, build
 * build the installer
 * install
 * run it
 * push the build results to freenet (using the node just started in the
   previous step) (not yet)

#### Targets:
 * build_utils  
    build tools required to build foe (ant tasks)
 * eclipse (not yet)  
    Build from eclipse workspace/local build.
 * github  
    Fetch/update sources from git(hub) and build
 * freenet (not yet)  
    Fetch/update sources from freenet and build
 * origin (not yet)  
    Fetch/update sources from origin (convert scm to git if needed) and build
 * patchmaker (not yet)  
    Generates a patch(set) to turn fred official/staging into the foe version

#### More Targets
 * make_readme
    Copy this helptext to README.md. Run this after updating this helptext.

#### Quick HOWTO:
 * type `ant github`
 * do `cd testnode`
 * run `./run.sh start` (or `java -cp org.eclipse.concierge.jar:wrapper.jar org.eclipse.concierge.ConciergeWrapper`)
    on succes the ports on 127.0.0.1 are 9999 (fproxy fred), 9998 (fcp), 9876 (new web ui)
Good luck!

Main targets:

 build_utils  --> build the buildutils
 eclipse      --> build from eclipse workspace
 freenet      --> clone/update sources from freenet
 github       --> clone/update sources from git(hub)
 help         --> diplay this project help
 origin       --> import to git/update all non git origin sources
Default target: help

BUILD SUCCESSFUL
Total time: 0 seconds
