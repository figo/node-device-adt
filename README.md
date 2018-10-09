# Node Device Advertiser
Advertise devices ( e.x GPU ) in nodes by adding node labels, so that 
pod can express device requirement through nodeSelector. 


## run model
there are two execution models we are exploring:

### run as daemonset
compiled it into go binary, then run as DaemonSet, 
it retrieve information on each node seperately.

### integrate with CCM 
integrate with cloud-controller-mananger (cloud provider) to
retrieve node devices and add label for all nodes in a central way.

